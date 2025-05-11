# CI/CD Pipeline - Escola App

Este repositório contém as configurações de CI/CD para o projeto Escola App, que consiste em uma aplicação frontend e backend.

## Estrutura do Projeto

- `frontend/`: Configurações de CI/CD para o frontend (Angular)
- `backend/`: Configurações de CI/CD para o backend (Spring Boot)

## Workflows

### Frontend
- Build e teste da aplicação Angular
- Push da imagem Docker para o DockerHub
- Deploy automático

### Backend
- Build e teste da aplicação Spring Boot
- Push da imagem Docker para o DockerHub
- Deploy automático

## Requisitos

- GitHub Actions
- DockerHub
- Acesso aos repositórios:
  - Frontend: carlinhoshk/escola-frontend
  - Backend: carlinhoshk/escola-app

## Configuração

1. Configure as secrets no GitHub:
   - `DOCKERHUB_USERNAME`
   - `DOCKERHUB_TOKEN`
   - `SSH_PRIVATE_KEY`
   - `SSH_HOST`
   - `SSH_USERNAME`

2. Certifique-se de que os repositórios frontend e backend estão configurados corretamente com seus respectivos Dockerfiles.

## Uso

Os workflows são executados automaticamente quando há push para as branches principais dos repositórios frontend e backend. 