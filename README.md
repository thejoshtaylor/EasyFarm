# EasyFarm 🐓

## Technology Stack and Features

- ⚡ [**FastAPI**](https://fastapi.tiangolo.com) for the Python backend API.
  - 🧰 [SQLModel](https://sqlmodel.tiangolo.com) for the Python SQL database interactions (ORM).
  - 🔍 [Pydantic](https://docs.pydantic.dev), used by FastAPI, for the data validation and settings management.
  - 💾 [PostgreSQL](https://www.postgresql.org) as the SQL database.
- 🚀 [React](https://react.dev) for the frontend.
  - 💃 Using TypeScript, hooks, [Vite](https://vitejs.dev), and other parts of a modern frontend stack.
  - 🎨 [Tailwind CSS](https://tailwindcss.com) and [shadcn/ui](https://ui.shadcn.com) for the frontend components.
  - 🤖 An automatically generated frontend client.
  - 🧪 [Playwright](https://playwright.dev) for End-to-End testing.
  - 🦇 Dark mode support.
- 🐋 [Docker Compose](https://www.docker.com) for development and production.
- 🔒 Secure password hashing by default.
- 🔑 JWT (JSON Web Token) authentication.
- 📫 Email based password recovery.
- ✅ Tests with [Pytest](https://pytest.org).

## ⚠️ UPDATED PHOTOS COMING SOON

### Dashboard Login

[![API docs](img/login.png)](https://github.com/fastapi/full-stack-fastapi-template)

### Dashboard - Admin

[![API docs](img/dashboard.png)](https://github.com/fastapi/full-stack-fastapi-template)

### Dashboard - Items

[![API docs](img/dashboard-items.png)](https://github.com/fastapi/full-stack-fastapi-template)

### Dashboard - Dark Mode

[![API docs](img/dashboard-dark.png)](https://github.com/fastapi/full-stack-fastapi-template)

### Interactive API Documentation

[![API docs](img/docs.png)](https://github.com/fastapi/full-stack-fastapi-template)

## How To Use It

Everything is built on docker compose, so starting the project out is pretty simple.

1. Clone the repo
   ```bash
   git clone https://github.com/thejoshtaylor/EasyFarm.git
   ```
1. Duplicate `.env.example` and rename it to `.env` and fill out all relevant variables
   1. Generate two secret keys, one for `SECRET_KEY` and one for `POSTGRES_PASSWORD`
      ```bash
      python -c "import secrets; print(secrets.token_urlsafe(32))"
      ```
   1. [optional] Connect your SMTP server (checkout [Mailgun](https://mailgun.com)!)
1. Run:
   ```bash
   docker compose build
   docker compose up 
   ```

## Backend Development

Backend docs: [backend/README.md](./backend/README.md).

## Frontend Development

Frontend docs: [frontend/README.md](./frontend/README.md).

## License

EasyFarm is licensed under the terms of the MIT license. It is derived from the [Full Stack FastAPI Template](https://github.com/fastapi/full-stack-fastapi-template), which is also MIT-licensed.
