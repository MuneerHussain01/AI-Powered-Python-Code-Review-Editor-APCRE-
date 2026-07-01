**APCRE: **
Autonomous Private Code Reviewer and Educational Platform
APCRE is a next-generation, offline-first, and privacy-respecting hybrid AI assistant designed for automated code reviews, style auditing, security analysis, and interactive software engineering tutoring.


Unlike standard cloud-based coding assistants, APCRE runs entirely locally to guarantee 100% data privacy and intellectual property security for developers and organizations.

**👥 Author Information**
Author: Muneer Hussain
Institution: Department of Software Engineering, Faculty of Telecommunication and Information Engineering, University of Engineering and Technology (UET), Taxila

**Project Role:** Lead Software Engineer & Machine Learning Developer
**
🌟 Key Architecture & Features**

APCRE operates via a Local Hybrid AI Architecture combining three distinct layers of analysis:

Deterministic Layer (Static AST Rules-Engine)

Performs structural parsing using an Abstract Syntax Tree (AST).
Audits PEP 8 / PEP 257 standards and catches security flaws (e.g., hardcoded credentials, swallowed exceptions) in sub-millisecond execution times.
Predictive Layer (Hybrid Machine Learning Ensemble)

Extracts a 779-Dimensional Fused Feature Space (768-D semantic projections via CodeBERT + 11-D concrete syntactic features via Tree-Sitter AST depth metrics).
Feeds into a soft-voting ensemble classifier (Random Forest, MLP Neural Network, and Gradient Boosting) achieving an empirically validated 94.59% F1-Score in classifying complex design anti-patterns, coupling behaviors, and SOLID violations.
Generative Layer (Local Stateful LLM Tutor)

Integrates a local, quantized Llama-3-8B-Instruct (Q4_K_M) model coordinated offline via the Ollama framework.
Retains context boundaries dynamically using persisted session memory in SQLite database files (apcre_memory.db).
Runs an Autonomous Sandbox Coder Agent to test generated code locally, capturing runtime tracebacks and recursively self-healing execution blocks.

**🛠️ Tech Stack & Dependencies**

Frontend (Next.js)
Framework: Next.js (React)
State Management: Zustand
Animations: Framer Motion
Editor Integration: Monaco Editor
Styling: Tailwind CSS & PostCSS
Backend (Node.js & Python)
Server: Node.js, Express, Socket.io
AI/ML Engine: Python 3, PyTorch, Scikit-Learn, NumPy
Parser & Embedder: Tree-Sitter, CodeBERT
Conversational Core: Ollama (Llama-3-8B)
Database: SQLite3

**🚀 Getting Started**
Prerequisites
Node.js (v18+)
Python (3.8+)
Ollama (installed locally and running)
Pull the model: ollama pull llama3
Step 1: Run the Backend Services
Navigate to the backend folder:
cd backend
Install Node dependencies:
npm install
Start the Express & Socket.io server:
npm start
Configure and run the local Python AI API service (backend/ai-engine/apcre_api.py):
cd ai-engine
python apcre_api.py
Step 2: Run the Next.js Frontend Dashboard
Open a new terminal in the root directory (apcre-ui).
Install frontend packages:
npm install
Boot up the local development server:
npm run dev
Open the interface in your browser (https://6a3fa52df59c19ecef72f4cb--sage-kitsune-510d43.netlify.app/).

**📄 License**
This project is licensed under the MIT License.
