# Requisitos Funcionais:

# Gerenciamento de pacientes: 

* O sistema deve permitir o cadastro de novos pacientes, inclusão de informações pessoais, histórico médico, alergias, medicações em uso, cirurgias anteriores e outras informações relevantes. O sistema também deve permitir a atualização de informações de pacientes existentes.

# Agendamento de consultas: 

* O sistema deve permitir que o hospital agende consultas médicas com especialistas, permitindo a escolha do médico, data e horário. O paciente deve ser notificado via e-mail ou mensagem de texto sobre sua consulta marcada.

# Gerenciamento de internações: 

* O sistema deve permitir a reserva de leitos para pacientes internados, bem como o registro de informações como horário de entrada, diagnóstico médico, medicamentos prescritos, tratamentos realizados e horário de saída. O sistema deve enviar alertas quando o paciente estiver próximo da alta hospitalar.

# Gerenciamento de alta hospitalar: 

* O sistema deve permitir que a equipe médica registre a alta hospitalar do paciente, informando a data e horário, medicamentos prescritos, orientações para acompanhamento médico posterior e outras informações relevantes.

# Gestão de usuários: 

* O sistema deve permitir o cadastro e gerenciamento de usuários, definindo perfis de acesso e níveis de permissão para cada usuário.

# Segurança de dados: 

* O sistema deve garantir a segurança dos dados dos pacientes e informações do hospital, implementando medidas de segurança como criptografia de dados, autenticação de usuários e backups regulares.

# Relatórios e estatísticas: 

* O sistema deve permitir a geração de relatórios e estatísticas sobre o número de pacientes atendidos, número de consultas agendadas, número de internações e outros dados relevantes.

# Registro de exames: 

* O sistema deve permitir o registro de exames realizados pelos pacientes, incluindo o tipo de exame, data de realização, resultados e observações.

# Prescrição de medicamentos: 

* O sistema deve permitir que os médicos prescrevam medicamentos aos pacientes, com informações detalhadas sobre o medicamento, posologia, duração do tratamento e contraindicações.

# Agenda de cirurgias: 

* O sistema deve permitir o agendamento de cirurgias, com informações sobre a data e horário, equipe médica envolvida, equipamentos necessários e outros detalhes relevantes.

# Acompanhamento pós-cirúrgico: 

* O sistema deve permitir o registro de informações sobre o acompanhamento pós-cirúrgico dos pacientes, com informações sobre medicações prescritas, instruções para cuidados em casa, consultas de acompanhamento e outros detalhes relevantes.

# Integração com prontuário eletrônico: 

* O sistema deve permitir a integração com o prontuário eletrônico dos pacientes, permitindo que os médicos acessem informações sobre o histórico médico dos pacientes, alergias, medicações em uso e outras informações relevantes.

# Notificação de pacientes: 

* O sistema deve permitir a notificação dos pacientes por e-mail, mensagem de texto ou outros meios de comunicação, com informações sobre consultas agendadas, resultados de exames, alta hospitalar e outras informações relevantes.

# Controle de acesso: 

* O sistema deve permitir o controle de acesso baseado em perfis de usuário e níveis de permissão, garantindo que apenas usuários autorizados tenham acesso às informações dos pacientes e aos serviços do sistema.

# ARQUITETURA

O sistema teria 6 serviços principais:

* Atendimento ao Paciente: responsável pelo cadastro de pacientes, agendamento de consultas e gerenciamento de internações.

* Pós-Atendimento: responsável pelo gerenciamento de alta hospitalar e acompanhamento pós-cirúrgico.

* Segurança e Acesso: responsável pela gestão de usuários, controle de acesso e segurança de dados.

* Prescrição e Exames: responsável pelo registro de exames e prescrição de medicamentos.

* Agenda de Cirurgias: responsável pelo agendamento de cirurgias.

* Comunicação e Informação: responsável pela integração com prontuário eletrônico e notificação de pacientes.

# Arquitetura Orientada a Eventos:

# Atendimento ao Paciente: 

Pode se comunicar com o serviço de Comunicação e Informação para notificar o paciente sobre consultas agendadas e resultados de exames.

# Pós-Atendimento: 

Pode se comunicar com o serviço de Atendimento ao Paciente para receber informações sobre internações e alta hospitalar.

# Prescrição e Exames: 

Pode se comunicar com o serviço de Atendimento ao Paciente para receber informações sobre o histórico médico do paciente e com o serviço de Comunicação e Informação para notificar o paciente sobre resultados de exames.

# Agenda de Cirurgias: 

Pode se comunicar com o serviço de Atendimento ao Paciente para receber informações sobre internações e com o serviço de Comunicação e Informação para notificar o paciente sobre a data e horário da cirurgia.

# Arquitetura Orientada a Microsserviços:

# Atendimento ao Paciente: 

Pode se comunicar com o serviço de Pós-Atendimento para enviar informações sobre internações e alta hospitalar. Também pode se comunicar com o serviço de Prescrição e Exames para registrar informações sobre o histórico médico do paciente.

# Pós-Atendimento: 

Pode se comunicar com o serviço de Atendimento ao Paciente para receber informações sobre pacientes internados. Também pode se comunicar com o serviço de Segurança e Acesso para gerenciar os perfis de acesso dos usuários envolvidos no processo de alta hospitalar.

# Segurança e Acesso: 

Pode se comunicar com todos os serviços para gerenciar os perfis de acesso dos usuários e garantir a segurança dos dados.

# Prescrição e Exames: 

Pode se comunicar com o serviço de Atendimento ao Paciente para receber informações sobre o histórico médico do paciente. Também pode se comunicar com o serviço de Comunicação e Informação para notificar o paciente sobre resultados de exames.

# Agenda de Cirurgias: 

Pode se comunicar com o serviço de Atendimento ao Paciente para receber informações sobre pacientes internados. Também pode se comunicar com o serviço de Comunicação e Informação para notificar o paciente sobre a data e horário da cirurgia.