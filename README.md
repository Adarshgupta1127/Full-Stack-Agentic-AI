# Full-Stack-Agentic-AI
📌 Features

Agentic AI Code Search – Search codebases using natural language queries.

Context-Aware Navigation – Understands repository structure & dependencies.

Full Stack Code Analysis – Works with frontend, backend, and database layers.

AI-Powered Documentation – Auto-generates explanations for code snippets & modules.

Feature Discovery Mode – Find where a specific functionality is implemented.

VS Code Integration – Native UI experience inside VS Code editor.

Multiple Code Repositories Support – Switch between projects effortlessly.

🛠️ Tech Stack
Layer	Technologies Used
Frontend	React, TailwindCSS, TypeScript
Backend	Node.js, Express.js
AI Layer	OpenAI GPT-4o / GPT-5 API, LangChain
Database	PostgreSQL (code metadata), Pinecone/Weaviate (vector DB)
Extension API	VS Code Extension API
Deployment	Vercel (frontend), Railway/Render (backend)
📂 Folder Structure
.
├── extension/           # VS Code extension source code
├── backend/             # Node.js + Express API
├── frontend/            # React + Tailwind UI (Webview)
├── scripts/             # Data ingestion & indexing scripts
├── docs/                # Documentation & architecture diagrams
└── README.md

⚙️ Installation & Setup
1️⃣ Clone the Repository
git clone https://github.com/your-username/agentic-ai-vscode-extension.git
cd agentic-ai-vscode-extension

2️⃣ Install Dependencies
cd backend && npm install
cd ../frontend && npm install
cd ../extension && npm install

3️⃣ Configure Environment Variables

Create a .env file in backend/ with:

OPENAI_API_KEY=your_openai_key
DATABASE_URL=postgres_connection_string
VECTOR_DB_URL=pinecone/weaviate_endpoint

4️⃣ Run the Development Servers
# Backend
cd backend && npm run dev

# Frontend
cd ../frontend && npm run dev

# VS Code Extension
cd ../extension && npm run watch

💡 Usage

Open VS Code & load your project.

Open the AI Code Search panel from the sidebar.

Enter a natural language query (e.g., "Where is user authentication handled?").

View results with highlighted matches & AI-generated explanations.

Click on any result to jump directly to the file and line number.

📊 Architecture Diagram
[ VS Code Extension ]
         |
         v
[ React Webview UI ] <--> [ Node.js Backend API ]
         |
         v
[ Vector DB (Pinecone) + PostgreSQL ] <--> [ OpenAI GPT + LangChain ]

🛠️ Future Improvements

Offline AI Mode using local LLMs.

Refactoring Suggestions for improving legacy code.

Integration with GitHub/GitLab APIs for live repo analysis.

Advanced Semantic Search using hybrid BM25 + embeddings.

🤝 Contributing

Pull requests are welcome! Please open an issue first to discuss major changes.

📜 License

MIT License – feel free to use and modify with attribution.
