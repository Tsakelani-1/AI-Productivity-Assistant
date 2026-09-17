# AI-Productivity-Assistant
AI-powered workplace assistant for email generation, meeting summaries, task planning, research assistance, and workplace chatbot interaction.
 1. Project objective
This project is a practical AI-powered workplace assistant designed to automate common professional tasks while demonstrating effective AI use, prompt engineering, responsible AI practices, and practical productivity value.

The project brief requires at least **three** core features. This solution demonstrates **all five**:
1. Smart Email Generator
2. Meeting Notes Summarizer
3. AI Task Planner / Scheduler
4. AI Research Assistant
5. AI Chatbot Interface

The brief describes the core goal as solving real-world workplace problems with AI. fileciteturn8file0L17-L37

## 2. How to run the prototype
```bash
npm install
npm run dev
```

The browser prototype includes **Demo Mode**, so it can be demonstrated without an API key.

## 3. Optional live AI integration
`api/generate.js` contains an optional server-side AI endpoint. If deployed, configure `OPENAI_API_KEY` as a server-side secret. Never expose a private API key in frontend code or commit it to GitHub.

## 4. Prompt engineering
The project uses a reusable framework:

**Role → Task → Context → Constraints → Output → Quality check**

Prompt templates are provided in `prompts/`. The approach reflects the brief's emphasis on designing, testing and refining effective prompts and comparing outputs for accuracy. fileciteturn8file0L67-L77

## 5. Responsible AI
The prototype encourages:
- Human review before important decisions or communications
- Protection of confidential information
- Verification of important facts
- Awareness of AI limitations and possible incorrect outputs
- Secure handling of API credentials

These safeguards align with the brief's requirement to identify limitations, bias and risks and include disclaimers and validation steps. fileciteturn8file0L75-L77

## 6. Project structure
```text
AI-Productivity-Assistant/
├── README.md
├── package.json
├── vite.config.ts
├── tsconfig.json
├── .env.example
├── index.html
├── src/
│   ├── main.tsx
│   ├── App.tsx
│   └── styles.css
├── api/
│   └── generate.js
├── prompts/
│   ├── email-prompts.md
│   ├── meeting-summary-prompts.md
│   ├── task-planning-prompts.md
│   └── research-prompts.md
├── documentation/
│   ├── project-overview.md
│   ├── project-documentation.pdf
│   ├── prompt-engineering.md
│   ├── responsible-ai.md
│   └── testing-results.md
├── presentation/
│   └── AI-Productivity-Assistant-Presentation.pptx
└── submission-checklist.md
```
