# AI-Assessment

## Assessment 1: Mini RAG Pipeline with ChromaDB on Colab

### Instructions:
1. Use Google Colab for the task.
2. Take 5–10 short documents (you can hardcode them).
3. Preprocess them using basic NLP (tokenization, stopword removal, etc.).
4. Embed the documents using the `sentence-transformers` library.
5. Store the embeddings in **ChromaDB** or **FAISS**.
6. Accept a user query and retrieve the top 2 most relevant documents based on semantic similarity.
7. Use a **HuggingFace LLM** (e.g., distilGPT2 or any open LLM) to generate an answer combining the retrieved documents.

---

## Assessment 2: Knowledge Graph + Semantic Search + QA

### Instructions:
1. Build a small **RDF knowledge graph** using the `rdflib` library.
   - Example: Alice knows Bob, Bob works at Google, Google is a company.
2. Convert the RDF triples into text format (e.g., "Alice knows Bob").
3. Embed those text sentences using `sentence-transformers`.
4. Store the embeddings in **FAISS**.
5. Accept a user query like: *"Where does Bob work?"*
6. Retrieve the most relevant sentence from the embeddings and use it to answer the query using a small LLM (e.g., `tiiuae/falcon-rw-1b` or `distilgpt2`).
