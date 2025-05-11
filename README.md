# CI/CD Pipeline - Escola App

Este repositório contém as configurações de produção para o projeto Escola App.

## Estrutura do Projeto

- `docker-compose.prod.yml`: Configuração de produção com Docker Compose
- `.github/workflows/`: Configurações de deploy em produção

## Configuração

1. Configure as secrets no GitHub:
   - `DOCKERHUB_USERNAME`
   - `DOCKERHUB_TOKEN`
   - `SSH_PRIVATE_KEY`
   - `SSH_HOST`
   - `SSH_USERNAME`

2. Certifique-se de que os repositórios frontend e backend estão configurados corretamente com seus respectivos Dockerfiles.

## Uso

O deploy em produção é acionado automaticamente quando há sucesso nos workflows de CI/CD dos repositórios:
- Frontend: carlinhoshk/escola-frontend
- Backend: carlinhoshk/escola-app

## Serviços

### Backend
- Porta: 9090
- Imagem: carlinhoshk/escola-app:latest

### Frontend
- Porta: 4200
- Imagem: carlinhoshk/escola-frontend:latest

### Banco de Dados
- MariaDB 10.11
- Porta: 3306
- Volume: mariadb_data 