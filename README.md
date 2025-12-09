
```markdown
# ✅ Knowledge Nexus - Multimodal RAG AI Assistant

A fully functional **Retrieval-Augmented Generation (RAG) AI Assistant** built on **Base44**, featuring a **glassmorphic design**, multi-agent AI orchestration, document ingestion, semantic search, and live AI-powered chat. This project is fully **production-ready**, optimized for Base44's infrastructure, and uses only **free & open-source AI tools**.

---

## 🌐 Project Links

- **Base44 Workspace (Editor):** [Click Here](https://app.base44.com/apps/690e11590409ef3e39eba392/editor/preview/chat)  
- **Deployed Application:** [Click Here](https://knowledge-nexus-39eba392.base44.app)  

---

## 🎯 Project Goal

Build a **modern, full-stack RAG system** for knowledge management and AI-powered Q&A with:

- Document ingestion from PDFs, DOCX, TXT, CSV, URLs, YouTube transcripts, and image OCR
- Multi-agent AI system for query understanding, retrieval, summarization, hallucination prevention, and citation enforcement
- Semantic and hybrid search with contextual relevance scoring
- Glassmorphic frontend with frosted glass effects, gradients, and dark/light mode
- Real-time chat with live streaming responses, retrieved chunk previews, and feedback (upvote/downvote)
- Admin dashboard for analytics, query logs, and feedback tracking

---

## 🎨 UI / UX Design

The UI is built with **Glassmorphism principles**:

- Frosted glass panels with backdrop blur (`backdrop-blur` CSS)
- Transparent UI elements with subtle 1px borders
- Layered translucent components for depth
- Vibrant gradient backgrounds (purple/blue/pink palette)
- Dark/light mode toggle
- Smooth animations and micro-interactions
- Document viewer panel for uploaded files
- Citation panel in chat interface

---

## ⚙️ Features

### Document Ingestion

- PDF, DOCX, TXT, CSV support
- Web URL scraping
- YouTube transcript extraction
- Image OCR (PaddleOCR/Tesseract)
- Auto-cleaning, chunking, metadata tagging
- RecursiveTextSplitter and auto-indexing agent

### RAG Pipeline

- Semantic and hybrid search
- Query understanding agent
- Retrieval agent
- Context compression agent
- Multi-step reasoning
- Hallucination prevention agent
- Citation enforcement agent
- Feedback loop (upvote/downvote)
- Weekly vector refresh (simulated in Base44)

### AI Agents

- **Router Agent:** Chooses the correct task
- **Retrieval Agent:** Fetches top-k relevant chunks
- **Ranking Agent:** Re-ranks results
- **Summarization Agent:** Compresses long texts
- **Verification Agent:** Validates hallucinations
- **Tool Agent:** OCR, web scraping, Python tools
- **Reasoner Agent:** Produces final answer
- **Context Compressor:** Condenses retrieved info
- **Citation Enforcer:** Adds proper citations

### Chat & Dashboard

- Multi-turn memory chat interface
- Live streaming AI responses
- Chunk preview and source citations
- Document upload & management page
- Admin dashboard with query logs, feedback analytics, vector DB usage

---

## 🏗️ Project Structure

```

/frontend
├─ components
├─ hooks
├─ pages
├─ services
└─ utils

/backend
├─ main.py
├─ routers/
├─ agents/
├─ services/
├─ rag/
├─ embeddings/
├─ vector_store/
├─ ocr/
├─ knowledge_graph/
├─ scheduler/
└─ tools/

/models       # LLM + embeddings
/uploads
/indexed
/docs

```

---

## 🔌 API Endpoints

- `/api/upload` — File upload
- `/api/index` — Process & chunk documents
- `/api/query` — RAG query endpoint
- `/api/retrieve` — Raw retrieval
- `/api/inspect/:id` — View retrieved chunks
- `/api/health` — Server health
- `/ws/chat` — WebSocket LLM streaming
- OCR, Web Scraper, YouTube Transcript endpoints

> ⚠️ On Base44, backend is adapted using **Base44 agents** and entity models instead of Python/FastAPI.

---

## 🚀 Getting Started

1. Open the **[Base44 workspace](https://app.base44.com/apps/690e11590409ef3e39eba392/editor/preview/chat)**.
2. Deploy directly via Base44 to access the live **[app](https://knowledge-nexus-39eba392.base44.app)**.
3. Upload documents in `Documents` page and let the system auto-index.
4. Use the **Chat page** to interact with AI agents.
5. Track analytics and feedback in the **Admin Dashboard**.

---

## 🛠️ Technology Stack

- **Frontend:** React + Vite, Tailwind CSS, ShadCN components, Glassmorphic design
- **Backend:** Base44 agent system & entity database
- **Vector DB / Memory:** Base44 entities for document chunks, conversation, and query logs
- **LLM Integration:** Base44 InvokeLLM (supports multi-turn memory, reasoning)
- **AI Tools:** OCR (PaddleOCR/Tesseract), web scraping, YouTube transcript fetching
- **Design:** Frosted glass, gradients, dark/light mode

---

## ⚡ Highlights

- Fully functional **RAG system** with multi-agent orchestration
- **Beautiful glassmorphic UI** with gradients and transparency
- Multi-modal ingestion: text, PDFs, DOCX, CSV, images, URLs, YouTube transcripts
- **Live chat streaming** with memory, citations, and feedback
- **Analytics dashboard** for admin insights
- Fully **production-ready** on Base44

---
