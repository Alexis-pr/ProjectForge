/projectforge                 <-- ROOT del repositorio
│
├── .github/                  <-- (DevOps) Workflows de CI/CD, Plantillas de Issues
│   └── workflows/
│       └── ci-pipeline.yml
│
├── docs/                     <-- (Transversal) Documentación compartida
│   ├── technical-design.pdf  <-- (Persona 1 + Equipo) Arquitectura, UML
│   ├── user-stories.md       <-- Historias de usuario
│   └── pitch-deck/           <-- PPTs y guiones
│
├── frontend/                 <-- (Persona 4) React App
│   ├── public/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   └── services/         <-- Axios clients
│   ├── package.json
│   ├── Dockerfile            <-- Dockerfile específico para React
│   └── .env.example
│
├── backend/                  <-- (Persona 1) ASP.NET Core API
│   ├── ProjectForge.Api/     <-- Punto de entrada (Program.cs)
│   ├── ProjectForge.Core/    <-- Entidades y Dominio
│   ├── ProjectForge.Infrastructure/ <-- DB Context (PostgreSQL)
│   ├── ProjectForge.sln      <-- Solución Visual Studio
│   ├── Dockerfile            <-- Dockerfile específico para .NET
│   └── appsettings.json
│
├── ai-service/               <-- (Persona 2) Python FastAPI
│   ├── app/
│   │   ├── api/              <-- Routers (endpoints)
│   │   ├── core/             <-- Config y seguridad
│   │   └── services/         <-- LLM Logic (OpenAI/Gemini)
│   ├── main.py
│   ├── requirements.txt
│   ├── Dockerfile            <-- Dockerfile específico para Python
│   └── .env.example
│
├── docker-compose.yml        <-- (DevOps) Orquestador Maestro
├── .gitignore                <-- Ignorar node_modules, bin, obj, __pycache__
└── README.md                 <-- Instrucciones de setup (Docker Compose Up)