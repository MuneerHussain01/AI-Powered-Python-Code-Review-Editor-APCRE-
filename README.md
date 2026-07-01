# APCRE – Autonomous Private Code Reviewer and Educational Platform

APCRE (Autonomous Private Code Reviewer and Educational Platform) is a next-generation, offline-first, and privacy-focused AI-powered software engineering platform designed for automated code review, security auditing, architecture analysis, and intelligent programming assistance.

Unlike traditional cloud-based coding assistants, APCRE runs entirely on local infrastructure, ensuring complete data privacy and intellectual property protection for developers, researchers, and organizations.

---

## 👨‍💻 Author

**Muneer Hussain**

- Department of Software Engineering
- Faculty of Telecommunication and Information Engineering
- University of Engineering and Technology (UET), Taxila
- Role: Lead Software Engineer & Machine Learning Developer

---

# 🚀 Key Features

- 🔒 100% Offline AI-powered Code Review
- 🔍 Static Code Analysis using Python AST
- 🛡️ Security Vulnerability Detection
- 📐 Software Architecture Review
- 📊 Machine Learning-based Code Quality Prediction
- 🤖 Local LLM Programming Assistant
- 🧠 Persistent Conversation Memory
- 💻 Interactive Code Editor
- 📈 Repository Intelligence
- 🎯 Automated Design Pattern & SOLID Principle Analysis

---

# 🏗️ System Architecture

APCRE is built upon a **three-layer Hybrid AI Architecture**.

## 1. Deterministic Layer (Static Analysis Engine)

This layer performs fast static code analysis using Python's Abstract Syntax Tree (AST).

Features include:

- PEP 8 Style Checking
- PEP 257 Documentation Analysis
- Code Smell Detection
- Hardcoded Credential Detection
- Exception Handling Analysis
- Security Rule Enforcement

Execution time is typically within milliseconds.

---

## 2. Predictive Layer (Machine Learning Engine)

The predictive engine combines semantic and syntactic code understanding using a hybrid feature representation.

### Feature Extraction

- 768-dimensional semantic embeddings using CodeBERT
- 11 handcrafted syntactic metrics extracted using Tree-Sitter

Total Feature Space:

**779 Dimensions**

### Machine Learning Models

- Random Forest
- Multi-Layer Perceptron (MLP)
- Gradient Boosting

The models are combined using a Soft Voting Ensemble.

### Performance

- F1 Score: **94.59%**

The model predicts:

- Design Anti-patterns
- SOLID Principle Violations
- Coupling Issues
- Architecture Smells

---

## 3. Generative Layer (Local AI Tutor)

The intelligent assistant operates entirely offline using:

- Llama-3-8B-Instruct (Q4_K_M)
- Ollama

Capabilities include:

- Code Explanation
- Bug Fix Suggestions
- Architecture Guidance
- Interactive Programming Tutor
- Stateful Conversations
- Automatic Code Execution
- Sandbox Testing
- Self-Healing Execution Loops

Conversation history is stored locally using SQLite.

---

# 🛠️ Technology Stack

## Frontend

- Next.js
- React
- Zustand
- Tailwind CSS
- Framer Motion
- Monaco Editor

## Backend

- Node.js
- Express.js
- Socket.io

## AI & Machine Learning

- Python 3
- PyTorch
- Scikit-Learn
- NumPy
- Tree-Sitter
- CodeBERT
- Ollama
- Llama 3

## Database

- SQLite3

---

# 📂 Project Structure

```
APCRE/
│
├── backend/
│   ├── ai-engine/
│   ├── workspace/
│   ├── server.js
│   └── package.json
│
├── src/
│   ├── app/
│   ├── components/
│   ├── learning/
│   └── store/
│
├── public/
├── scratch/
├── package.json
└── README.md
```

---

# 🚀 Getting Started

## Prerequisites

- Node.js 18+
- Python 3.8+
- Ollama

Install the required model:

```bash
ollama pull llama3
```

---

## Backend Setup

Navigate to the backend directory:

```bash
cd backend
```

Install dependencies:

```bash
npm install
```

Start the backend server:

```bash
npm start
```

Open another terminal:

```bash
cd backend/ai-engine
```

Run the AI API:

```bash
python apcre_api.py
```

---

## Frontend Setup

Return to the project root:

```bash
npm install
```

Start the Next.js application:

```bash
npm run dev
```

Open your browser:

```
http://localhost:3000
```

---

# 🎯 Core Modules

- AI Code Reviewer
- Security Scanner
- Architecture Analyzer
- Repository Intelligence
- Interview Assistant
- Research Assistant
- Knowledge Graph
- Test Generator
- Autonomous Coding Agent
- Interactive Learning Platform

---

# 🔒 Privacy

APCRE is designed with privacy as its primary objective.

- No cloud dependency
- No source code leaves the user's computer
- Fully offline AI inference
- Local databases only
- Local LLM execution through Ollama

---

# 📈 Machine Learning Highlights

- CodeBERT Semantic Embeddings
- Tree-Sitter Structural Features
- Ensemble Learning
- Software Defect Prediction
- Design Smell Detection
- Architecture Quality Analysis

---

# 📄 License

This project is licensed under the **MIT License**.

---

# ⭐ Acknowledgements

This project was developed as part of academic research in Software Engineering at:

**Department of Software Engineering**

**Faculty of Telecommunication and Information Engineering**

**University of Engineering and Technology (UET), Taxila**

---

## 👨‍💻 Developer

**Muneer Hussain**

Lead Software Engineer • Machine Learning Developer • Software Engineering Researcher

---

⭐ If you find this project useful, consider giving it a **Star** on GitHub.
