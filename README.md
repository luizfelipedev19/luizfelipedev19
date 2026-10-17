# Luiz Felipe Vieira

**Desenvolvedor Backend Júnior | PHP e Node.js**

Atuo como desenvolvedor backend júnior na Allenda, plataforma multitenant, trabalhando na manutenção e evolução de sistemas em produção, no desenvolvimento de funcionalidades e na integração entre aplicações. Curso Análise e Desenvolvimento de Sistemas na FATEC Mococa e desenvolvo projetos próprios com PHP, JavaScript e Node.js.

Minha experiência inclui APIs REST, integração com sistemas legados, automação de rotinas e persistência em bancos de dados. No ambiente profissional, utilizo Docker, Kubernetes e Argo CD em atividades relacionadas a ambientes e processos de entrega de aplicações.

Tenho interesse em segurança de aplicações, arquitetura de software e organização de regras de negócio. Nos projetos, aplico autenticação e autorização com JWT, API Keys e HMAC, além de explorar arquitetura MVC, organização em camadas e arquitetura hexagonal.

## Tecnologias e conhecimentos

### Desenvolvimento e bancos de dados

<img align="left" alt="PHP" title="PHP" width="30px" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/php/php-original.svg" />
<img align="left" alt="Node.js" title="Node.js" width="30px" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/nodejs/nodejs-original.svg" />
<img align="left" alt="NestJS" title="NestJS" width="30px" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/nestjs/nestjs-original.svg" />
<img align="left" alt="MySQL" title="MySQL" width="30px" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/mysql/mysql-original.svg" />
<img align="left" alt="PostgreSQL" title="PostgreSQL" width="30px" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/postgresql/postgresql-original.svg" />
<img align="left" alt="MongoDB — aprendizado inicial" title="MongoDB — aprendizado inicial" width="30px" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/mongodb/mongodb-original.svg" />
<img align="left" alt="JavaScript" title="JavaScript" width="30px" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/javascript/javascript-original.svg" />
<img align="left" alt="HTML5" title="HTML5" width="30px" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/html5/html5-original.svg" />
<img align="left" alt="CSS3" title="CSS3" width="30px" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/css3/css3-original.svg" />

<br/><br/>

### Infraestrutura e DevOps

<img align="left" alt="Docker" title="Docker" width="30px" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/docker/docker-original.svg" />
<img align="left" alt="Kubernetes" title="Kubernetes" width="30px" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/kubernetes/kubernetes-original.svg" />
<img align="left" alt="Argo CD" title="Argo CD" width="30px" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/argocd/argocd-original.svg" />

<br/><br/>

| Área | Tecnologias e práticas |
| --- | --- |
| Backend | PHP, Node.js, Express, NestJS e desenvolvimento de APIs REST. |
| Frontend | JavaScript, HTML5 e CSS3. |
| Bancos de dados | PostgreSQL e MySQL; aprendizado inicial de MongoDB aplicado ao projeto My-CEP. |
| Acesso a dados | PDO, Prisma e Mongoose. |
| Segurança | JWT, API Keys, HMAC e práticas de autenticação e autorização. |
| Arquitetura | MVC, arquitetura em camadas e estudos de arquitetura hexagonal. |
| Integrações | Consumo de APIs, integração com sistemas legados e envio de mensagens via WhatsApp. |
| Automação | Agendamento de rotinas com cron jobs. |
| Infraestrutura | Docker, Docker Compose, Kubernetes e Argo CD. |
| Versionamento e documentação | Git, GitHub e Swagger/OpenAPI. |

## Projetos em destaque

### Helpdesk API
Sistema de helpdesk multiempresa (multi-tenant), com backend em Node.js, Express e TypeScript, persistência em PostgreSQL e autenticação via JWT. Cada empresa cadastrada opera de forma isolada, com seus próprios usuários, categorias e chamados.

- Isolamento de dados por empresa (multi-tenancy) reforçado em todas as camadas de acesso ao banco.
- Autenticação com JWT e senhas com hash via Argon2, com papéis de usuário (atendente, gestor, admin) e autorização por rota.
- Fluxo completo de ciclo de vida de chamados: criação, atribuição a um atendente (ou fila sem responsável), atualização e trilha de auditoria das mudanças de status, prioridade e responsável.
- Rate limiting diferenciado por rota (login, cadastro de empresa, uso geral da API) para mitigar força bruta e abuso.
- Validação de entrada com Zod e tratamento de erros padronizado.
- Backend organizado em camadas (rotas, controllers, services, repositories, schemas e models), com transações de banco para garantir consistência entre atualização de dados e registro de auditoria.
- Ambiente containerizado com Docker Compose, incluindo banco PostgreSQL e sistema de migrations versionadas.
- Projeto em desenvolvimento ativo, com foco em arquitetura de backend, modelagem de domínio multi-tenant e boas práticas de segurança em APIs REST.

### My-CEP

Aplicação web para consulta de CEPs brasileiros, com interface responsiva em HTML, CSS e JavaScript e backend em Node.js com Express. A API consulta a ViaCEP e persiste os dados de endereço no MongoDB por meio do Mongoose.

- Validação e normalização de CEPs no frontend e no backend.
- Integração com um serviço externo para consulta de endereços.
- Persistência de endereço e data da consulta no MongoDB.
- Organização do backend em rotas, controller, serviço, modelo e configuração de banco de dados.
- Configuração por variáveis de ambiente e comunicação HTTP entre interface e API.

Projeto educacional voltado à prática de Node.js, integração entre frontend e backend e armazenamento de dados em banco não relacional.

### Rodízio — Igreja

Sistema para gerenciar escalas de avisos de uma igreja, com cadastro de pessoas, definição de horários e envio automático de lembretes pelo WhatsApp.

- Backend em PHP sem framework, com API REST, PDO e PostgreSQL.
- Autenticação com JWT e API Key.
- Frontend em PHP e JavaScript, atuando como BFF (Backend for Frontend).
- Agendamento de lembretes com cron.
- Integração com uma API externa para envio de mensagens pelo WhatsApp.
- Registro de auditoria das requisições da API.
- Ambiente containerizado com Docker Compose.

### App-Faturas

Sistema desenvolvido em PHP para organizar e enviar faturas conforme as regras de negócio da empresa, integrado à API de um sistema administrativo legado.

- Consumo de API de sistema legado desenvolvido em PHP.
- Regras de organização e formatação de faturas.
- Envio de faturas por WhatsApp e e-mail.
- Dashboard com indicadores e listagem paginada.
- Documentação da API com Swagger.

### Quick-Note

Extensão para Firefox desenvolvida em JavaScript para criação e gerenciamento de anotações rápidas.

- Utilização da WebExtensions API.
- Interface para criação e gerenciamento de notas.
- Persistência local dos dados.

## Experiência profissional

### Manutenção e evolução da Allenda

Atuação na manutenção e evolução da **Allenda**, plataforma multitenant desenvolvida com **NestJS**, no ecossistema Node.js. O sistema reúne integração com WhatsApp, helpdesk, CRM, automação de processos e funcionalidades de atendimento ao cliente para múltiplas organizações.

Contribuo para a correção de problemas e evolução das funcionalidades, aplicando boas práticas de desenvolvimento e arquitetura de software, com foco na separação de responsabilidades, organização das regras de negócio e manutenção do código.

- Manutenção e evolução de funcionalidades de atendimento integradas ao WhatsApp.
- Atuação em recursos de helpdesk, CRM e automação de processos.
- Desenvolvimento e manutenção do backend em NestJS.
- Aplicação de boas práticas na organização dos componentes e das regras de negócio.
- Atenção ao contexto de cada organização na evolução de um sistema multitenant.

### Manutenção e evolução de sistemas legados

Atuação na manutenção de um sistema empresarial desenvolvido em PHP 5.3 com MySQL, incluindo correção de problemas, implementação de funcionalidades e integração com aplicações mais recentes.

Essa experiência envolve compreender regras de negócio existentes, dar continuidade à operação dos sistemas e desenvolver melhorias para demandas do ambiente de telecomunicações.

## Projetos acadêmicos em Java

<img align="left" alt="Java" title="Java — formação acadêmica" width="30px" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/java/java-original.svg" />
<img align="left" alt="Spring" title="Spring" width="30px" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/spring/spring-original.svg" />

<br/><br/>

Estudo Java como parte da formação em Análise e Desenvolvimento de Sistemas. Os projetos com Spring Boot complementam o aprendizado de orientação a objetos, APIs REST, segurança e persistência de dados.

### API de Usuários

API REST para cadastro e autenticação de usuários, desenvolvida com Java 21 e Spring Boot 3.

- Autenticação JWT e proteção de endpoints com Spring Security.
- Persistência com Spring Data JPA, Hibernate e PostgreSQL.
- Versionamento do banco de dados com Flyway.
- Documentação interativa com Swagger/OpenAPI.
- Gerenciamento de dependências com Maven.

### API de Gerenciamento de Tarefas

API REST desenvolvida com Java 21 e Spring Boot 3.2.5 para gerenciamento de tarefas associadas ao usuário autenticado.

- Cadastro e autenticação de usuários com JWT.
- Criação, listagem, atualização de status e exclusão de tarefas.
- Proteção de rotas com Spring Security.
- Persistência com Spring Data JPA e Hibernate.
- Organização em controllers, services, repositories, DTOs e componentes de segurança.
- Tratamento global de exceções.

## Formação acadêmica

**Análise e Desenvolvimento de Sistemas — FATEC Mococa**  
Em andamento.

## Interesses de desenvolvimento

- Desenvolvimento backend com PHP e Node.js.
- Integração de sistemas e construção de APIs REST.
- Segurança, autenticação e autorização.
- Automação de processos e rotinas operacionais.
- Arquitetura de software, manutenção e evolução de aplicações.
