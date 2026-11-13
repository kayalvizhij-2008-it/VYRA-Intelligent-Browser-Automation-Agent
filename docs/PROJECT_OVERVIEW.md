# VYRA — Intelligent Browser Automation Agent

**Turn natural-language instructions into browser actions. Automate workflows. Stay in control.**

VYRA is an intelligent browser automation platform designed to simplify repetitive web tasks through natural-language instructions. It connects an interactive web interface with an AI-powered browser automation engine, enabling users to initiate workflows, monitor execution, and review automation history from one centralized workspace.

🌐 **Live Platform:** https://vyra-five-chi.vercel.app  
⚙️ **Backend API:** https://vyra-api-wpc0.onrender.com  
📦 **Repository:** https://github.com/kayalvizhij-2008-it/VYRA

---

## ✨ What is VYRA?

Modern digital workflows often require people to perform the same browser actions repeatedly: navigating websites, interacting with forms, collecting information, and completing multi-step processes.

VYRA aims to make these workflows easier.

Instead of manually carrying out every browser interaction, users can provide instructions in natural language and initiate an automation run through a centralized interface.

VYRA combines an AI-powered automation backend, browser execution infrastructure, and a modern frontend to make browser automation more accessible, observable, and manageable.

## 🚀 Key Features

### 🤖 Natural-Language Automation
- Describe browser tasks using natural-language instructions.
- Initiate automation runs through a dedicated interface.
- Connect supported AI providers to power automation.

### 🌐 Intelligent Browser Execution
- Built around the `browser-use` automation framework.
- Designed for browser-based task execution.
- Supports multi-step browser workflows through the automation engine.

### 📊 Centralized Dashboard
- Overview of automation activity.
- Dedicated automation creation interface.
- Organized run history and execution details.
- Browser and integration management sections.

### 📜 Run History & Monitoring
- View previous automation runs.
- Inspect individual run details.
- Track execution status and available run information.

### 🔌 Multi-Provider Architecture
- Provider selection through the automation interface.
- Configuration support for multiple AI model providers.
- Server-side credential configuration.
- Clear feedback when a provider requires configuration.

### 🎨 Modern User Experience
- Premium glass-inspired interface.
- Interactive 3D Fibre Arc and Glitter Cascade visual effects.
- Smooth transitions and polished page layouts.
- Responsive design for desktop and mobile screens.

## 🛠️ Technology Stack

| Layer | Technologies |
|---|---|
| Frontend | React, TypeScript, Vite |
| Styling | CSS, Glassmorphism, Responsive UI |
| Backend | Python, FastAPI |
| Automation Engine | browser-use 1.0.2 |
| Browser Runtime | Chromium |
| Data Storage | SQLite |
| Deployment | Vercel, Render |
| Containerization | Docker |

## 🏗️ System Architecture

VYRA follows a frontend-backend architecture that separates user interaction from automation execution.

```text
             USER
               |
               v
       VYRA WEB APPLICATION
         React + TypeScript
               |
               v
          FASTAPI SERVER
               |
       +-------+-------+
       |               |
       v               v
  AI PROVIDERS     RUN MANAGEMENT
       |               |
       +-------+-------+
               |
               v
       BROWSER AUTOMATION
          browser-use
               |
               v
           CHROMIUM
               |
               v
       EXECUTION RESULTS
               |
               v
        RUN HISTORY / UI
```

## 📁 Project Structure

```text
VYRA/
│
├── server/
│   ├── vyra/
│   │   ├── config.py
│   │   ├── app.py
│   │   └── ...
│   ├── .env.example
│   └── ...
│
├── web/
│   ├── src/
│   │   ├── pages/
│   │   ├── styles.css
│   │   └── ...
│   ├── vercel.json
│   └── ...
│
├── Dockerfile
├── .dockerignore
├── render.yaml
├── README.md
└── ...
```

## ⚙️ Getting Started

### Prerequisites

- Node.js and npm
- Python
- Git
- Chromium-compatible browser runtime
- API credentials for at least one supported AI provider

### 1. Clone the repository

```bash
git clone https://github.com/kayalvizhij-2008-it/VYRA.git
cd VYRA
```

### 2. Configure the backend

Navigate to the server directory and configure the environment using the supplied example file.

```bash
cd server
```

Create your local `.env` file and add the credentials for your chosen AI provider.

Example:

```env
OPENAI_API_KEY=your_api_key
```

Other supported provider configurations include Anthropic, Google/Gemini, Browser Use, and compatible model endpoints. Use the project's environment example for the exact configuration requirements.

Never commit API keys or private credentials.

### 3. Start the backend

Install the backend dependencies using the project's dependency configuration, then start the FastAPI application using its configured entry point.

### 4. Start the frontend

Open another terminal:

```bash
cd web
npm install
npm run dev
```

Open the local URL displayed by Vite in your browser.

## 🌍 Live Deployment

VYRA uses a separated deployment architecture:

- **Frontend:** Vercel
- **Backend:** Render
- **Browser execution:** Chromium-based runtime
- **API communication:** Frontend-to-backend HTTP requests

Production availability and automation execution depend on the backend service, configured provider credentials, and hosting resources.

## 🔐 Security & Configuration

- Keep API credentials on the server.
- Use environment variables for provider configuration.
- Do not expose secret keys in frontend code.
- Keep `.env` files out of version control.
- Configure production CORS origins appropriately.
- Use trusted provider credentials and secure deployment settings.

## 🧪 Project Validation

The development and deployment workflow has included:

- Frontend TypeScript validation.
- Production frontend builds.
- Backend API tests.
- Provider configuration tests.
- Production API health checks.
- Route and responsive-layout checks.

A successful deployment does not automatically mean every provider configuration or real-world automation workflow has been tested. Actual browser runs require a configured provider and a functioning browser runtime.

## 🔮 Future Scope

VYRA can evolve into a more comprehensive browser automation ecosystem through:

- Reusable automation templates.
- Scheduled and recurring workflows.
- Advanced execution analytics.
- Improved failure recovery and retry mechanisms.
- Secure credential management.
- More browser and integration capabilities.
- Team-based automation workspaces.
- Workflow export and sharing.

## 🎯 Vision

Our vision is to make browser automation more accessible by allowing people to focus on what they want to accomplish instead of repeatedly performing every browser interaction themselves.

**VYRA — From instructions to intelligent browser actions.**

---

## 👩‍💻 Author

**Kayalvizhi J**  
Information Technology  
Chennai Institute of Technology

## 📄 License

Choose and add an appropriate open-source license before distributing this project. Until then, no license is implied.
