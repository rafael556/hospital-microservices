# Stage 1: Build
FROM node:16-alpine AS build

# Criação do diretório da aplicação
WORKDIR /app

# Copia os arquivos do projeto para dentro do container
COPY . .

# Instala as dependências com o Yarn
RUN yarn install --frozen-lockfile --production=false

# Compila a aplicação
RUN yarn build

# Stage 2: Release
FROM node:16-alpine AS release

# Criação do diretório da aplicação
WORKDIR /app

# Copia os arquivos da build para dentro do container
COPY --from=build /app/dist ./dist
COPY --from=build /app/node_modules ./node_modules

# Cria um usuário não root para segurança do container
RUN addgroup -S appgroup && adduser -S appuser -G appgroup

# Define o usuário não root como dono do diretório da aplicação
RUN chown -R appuser:appgroup /app

# Define o usuário não root como usuário padrão
USER appuser

EXPOSE 8083

# Inicia a aplicação
CMD ["yarn", "start:prod"]
