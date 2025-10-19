# Movies Catalog 🎬

Catálogo de filmes desenvolvido com Ruby on Rails, PostgreSQL, JavaScript e Bootstrap.

## 🚀 Tecnologias

- Ruby 3.2.2
- Rails 7.1
- PostgreSQL 15
- Bootstrap 5
- Docker & Docker Compose

## 📋 Pré-requisitos

- Docker
- Docker Compose

## 🔧 Instalação e Execução

1. Clone o repositório:
```bash
git clone https://github.com/cesarka1/movies-catalog.git
cd movies-catalog
```

2. Copie o arquivo de exemplo de variáveis de ambiente:
```bash
cp .env.example .env
```

3. **IMPORTANTE**: Edite o arquivo `.env` e altere as senhas e credenciais:
```bash
# Edite estas variáveis com valores seguros:
POSTGRES_PASSWORD=sua_senha_segura_aqui
```

4. Construa e inicie os containers:
```bash
docker-compose build
docker-compose up
```

5. Acesse a aplicação em: http://localhost:3000

## 🔒 Segurança

- O arquivo `.env` contém informações sensíveis e **NÃO** é versionado no Git
- Use o `.env.example` como referência para criar seu `.env` local
- Em produção (Render), configure as variáveis de ambiente no painel do serviço

## 📦 Deploy no Render

1. Faça push do código para o GitHub
2. No Render, conecte o repositório
3. Configure as variáveis de ambiente no painel do Render:
   - `POSTGRES_USER`
   - `POSTGRES_PASSWORD`
   - `POSTGRES_DB`
   - `RAILS_ENV=production`

## 🛠️ Comandos Úteis

```bash
# Parar os containers
docker-compose down

# Reconstruir os containers
docker-compose build --no-cache

# Ver logs
docker-compose logs -f

# Executar comandos Rails
docker-compose run --rm web rails console
docker-compose run --rm web rails db:migrate
```

## 📝 Licença

Este projeto é de código aberto.
