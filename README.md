# Plataforma de Gestão de TCCs

Este projeto visa criar uma plataforma de código aberto que simplifica a gestão de Trabalhos de Conclusão de Curso (TCCs) para instituições de ensino, professores e estudantes. A plataforma oferece uma série de recursos e funcionalidades que tornam o processo de acompanhamento, avaliação e administração de TCCs mais eficiente e organizado.

## Projetos Relacionados

- [patrickbindelli/gestao-tcc-front](https://github.com/patrickbindelli/gestao-tcc-front) - Repositório contendo o código fonte da interface do usuário da plataforma de gestão de TCCs.
- [patrickbindelli/gestao-tcc-back](https://github.com/patrickbindelli/gestao-tcc-back.git) - Repositório contendo o código fonte do servidor e da lógica de negócios da plataforma de gestão de TCCs.

## Funcionalidades

- Gerenciamento de Alunos e Professores
- Acompanhamento de Progresso
- Controle de Documentação

## Variáveis de Ambiente

Para rodar esse projeto, você vai precisar adicionar as seguintes variáveis de ambiente no seu .env

### Arquivo `.env`:

Configurações da aplicação
| Variável | Exemplo |
| ------------- | ------------- |
| DEBUG | 0 ou 1 |
| SECRET_KEY | Este valor [a configuração SECRET_KEY] é a chave para garantir a segurança dos dados assinados. Exemplo: `J6NH8Y82qz6MoFc` |
| SQL_ENGINE | Seguir o modelo do [Django](https://docs.djangoproject.com/en/4.2/ref/databases/). Exemplo: `django.db.backends.postgresql`|
| SQL_DATABASE | Nome do banco de dados. Exemplo: `postgres` |
| SQL_USER | Nome do usuário do banco. Exemplo: `postgres` |
| SQL_PASSWORD | Senha do banco de dados. Exemplo: `postgres` |
| SQL_HOST | IP ou endereço do banco de dados. Exemplo: `db` para o container db |
| SQL_PORT | Porta do banco de dados. Exemplo: `5432` |
| DATABASE | Define o projeto está utilizando uma database. Exemplo: `postgres` |

### Arquivo `.env.db`:

Configurações do Banco de Dados embutido

| Variável          | Exemplo                                       |
| ----------------- | --------------------------------------------- |
| POSTGRES_USER     | Nome do usuário do banco. Exemplo: `postgres` |
| POSTGRES_PASSWORD | Senha do banco de dados. Exemplo: `postgres`  |
| POSTGRES_DB       | Nome do banco de dados. Exemplo: `postgres`   |

## Deploy

Para fazer o deploy desse projeto execute

```bash
  docker compose up -d --build
```

## Stack utilizada

**Front-end:** Typescript, NextJS

**Back-end:** Python, Django

## Licença

[MIT](https://choosealicense.com/licenses/mit/)
