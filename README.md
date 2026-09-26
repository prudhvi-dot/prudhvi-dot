🚀 DocuSense 2.0 — Smarter, Self-Correcting RAG

I’ve rebuilt my document chat app from the ground up. Beyond separating frontend and backend, the real leap is a redesigned RAG pipeline that doesn’t just retrieve — it evaluates, refines, and validates answers before responding.

🏗️ **New Architecture**

The application is now split into a dedicated frontend and backend:

🖥️ **Frontend**

• Next.js
• React
• Tailwind CSS
• Streaming chat responses

⚙️ **Backend**

• FastAPI
• SQLAlchemy
• PostgreSQL / Neon
• REST APIs
• Cookie-based authentication

🧠 **Redesigned RAG Pipeline**

Instead of the traditional:

**Query → Retrieve → Generate**

DocuSense now follows an iterative workflow built with LangGraph:

**Query → Route → Retrieve → Evaluate → Refine / Rewrite → Generate → Validate → Revise**

The workflow can:

🔹 Route the query between conversation and document-based questions

🔹 Retrieve relevant context from the document

🔹 Evaluate the quality of retrieved context

🔹 Refine the retrieved context when needed

🔹 Rewrite the query when retrieval isn't useful

🔹 Generate an answer using the retrieved context

🔹 Check whether the answer is sufficiently supported

🔹 Check whether the answer actually addresses the user's question

🔹 Revise and retry when necessary

🔹 Return a grounded response or indicate when an answer cannot be found

The goal was to move beyond a simple retrieve-and-generate approach and build a RAG system that can reason about its own retrieval and generated responses.

🛠️ **Tech Stack**

Next.js · FastAPI · LangChain · LangGraph · Pinecone · PostgreSQL · SQLAlchemy · OpenAI Embeddings

🌐 **Live Demo:**
https://docu-sense-2-0-wowt.vercel.app/

💻 **GitHub Repository:**
https://github.com/prudhvi-dot/DocuSense_2.0

This rebuild has been a great learning experience — especially understanding how much engineering goes into building reliable AI applications beyond simply connecting an LLM to a vector database.

**Retrieval → Evaluation → Routing → Refinement → Validation → Streaming → Persistence**

Still improving DocuSense step by step. 🚀

#AI #RAG #LangGraph #LangChain #FastAPI #NextJS #Pinecone #GenerativeAI #LLM #PostgreSQL #AIEngineering #SoftwareEngineering
