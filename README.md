# Nexus AI — AI-03 Frontend Prototype

A polished, responsive frontend prototype for the Topic-Augmented Knowledge Graph Builder problem statement.

## Run locally

Requirements: Node.js 20.19+ (or a compatible newer LTS release) and npm.

```bash
npm install
npm run dev
```

Open the local URL printed by Vite.

## Included in this prototype

- Responsive dark knowledge-workspace dashboard
- Interactive SVG knowledge graph with selectable nodes and relationship details
- Sample evidence library and evidence explorer modal
- Demo chat with sample answers and clickable evidence references
- Local file picker for PDF, TXT, and Markdown files
- Session-only file list with remove actions
- SVG graph export, node filtering, and zoom controls

## Important status note

This is the frontend prototype only. The graph, evidence passages, statistics, and chat answers are sample demo data. File selection currently adds files to the local session list; it does **not** upload, parse, embed, or store document contents. No backend, LLM, Neo4j, or ChromaDB connection is configured yet.

## Next integration stages

1. FastAPI backend and document upload/parse endpoints
2. Chunking, embeddings, and ChromaDB vector retrieval
3. Entity/relationship extraction and Neo4j graph persistence
4. Query router for thematic vs. local graph retrieval
5. LLM-generated answers grounded in retrieved passages and graph paths
6. Evaluation and tests for retrieval quality, citations, and hallucinations
