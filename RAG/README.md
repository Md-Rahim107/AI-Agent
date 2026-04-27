## RAG
A complete RAG implementation in n8n. The ingestion workflow chunks uploaded files (Google Drive → Recursive Text Splitter → Gemini Embeddings → Qdrant). The chat workflow uses Groq/Gemini + memory and always retrieves from Qdrant first before generating a response. Strict prompting ensures no hallucinations — if data is absent, it says so.


<img width="1162" height="643" alt="Company Document Insert Image (1)" src="https://github.com/user-attachments/assets/55b3d59b-2930-439f-ac62-a7a693571ec7" />
<img width="1629" height="843" alt="Company Document Insert Image (2)" src="https://github.com/user-attachments/assets/0b957b00-f1c2-4a52-9115-7e2580c8efea" />



