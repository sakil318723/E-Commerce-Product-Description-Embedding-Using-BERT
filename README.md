E-commerce Semantic Search with BERT

Real-time semantic search for e-commerce products using BERT embeddings and FAISS vector search. Understands natural language queries with 92-100% accuracy.

Features

· BERT-based semantic embeddings
· FAISS vector search (GPU optimized)
· 92-100% accuracy on test queries
· <50ms search latency
· Ready-to-use Flask API

Quick Start

```bash
# Install dependencies
pip install torch transformers faiss-gpu pandas

# Run Jupyter notebook
jupyter notebook ecommerce_bert_embeddings.ipynb
```

Usage

```python
# Search for products
results = search_engine.search_by_text("wireless headphones", k=5)

for result in results:
    print(f"Title: {result['product_info']['title']}")
    print(f"Similarity: {result['similarity_score']:.3f}")
```

API Deployment

```bash
cd ecommerce_search_export
python api_server.py
# API at http://localhost:5000/search
```

Results

· Category Accuracy: 100%
· Keyword Accuracy: 92%
· Search Speed: <50ms

Files

· ecommerce_bert_embeddings.ipynb - Complete implementation
· product_embeddings.npy - BERT embeddings
· faiss_index.bin - Vector search index
· api_server.py - Production API

---

Built with PyTorch, Transformers, and FAISS. 92-100% accuracy achieved.
