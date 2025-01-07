# **Recommendation using Small Language Models**

## **Project Overview**
This project focuses on building a **Recommendation System** that leverages **Small Language Models (SLMs)** to enhance the recommendation process inspired by **Agent-based Collaborative Filtering (Agent CF)**. By incorporating techniques from **Retrieval-Augmented Generation (RAG)** and employing **memory-based optimizations**, this system aims to improve personalization, handle cold-start problems, and provide cross-domain recommendations.

## **Key Features**
- **Agent-Based Interaction**: Autonomous interaction between user agents and item agents to simulate and rank recommendations dynamically.
- **Memory Management**: Use of long-term and short-term memory for contextual and evolving preference representations.
- **RAG Techniques**: Enhanced recommendations with query expansion, hypothetical embeddings, and re-ranking.
- **Cross-Domain Extrapolation**: Recommendations that leverage user preferences across different content domains (e.g., from movies to music).

## **Methodology**
1. **Collaborative Memory-Based Optimization**:
   - Iterative memory updates through user-item agent interactions.
   - Reflection-based learning without gradient updates (since the LLM remains fixed).
   
2. **Implicit Preference Propagation**:
   - Autonomous propagation of preferences between agents using individual memory reflections.
   
3. **Contrastive Learning**:
   - Training with pairs of positive and negative candidates to improve the discrimination of relevant items.

4. **Collaborative Reflection and Memory Update**:
   - The system updates agent memories based on the agent's decisions and explanations for their choices.

## **RAG Techniques Applied**
1. **HyDE (Hypothetical Document Embedding)**:
   - Generates hypothetical document embeddings to enrich query representations.
2. **Query Expansion**:
   - Enriches user and item descriptions by including semantic terms to improve retrieval accuracy.
3. **Iterative Retrieval**:
   - Refines queries over multiple steps based on user feedback to improve personalization.
4. **Contextual Retrieval**:
   - Leverages interaction history to provide context-aware retrieval and improve recommendation precision.
5. **Re-ranking Retrieved Information**:
   - Prioritizes retrieved items based on their contextual relevance and direct feedback.

## **Metrics**
The evaluation will use:
- **Precision@K** and **Recall@K** for ranking performance.
- **MRR (Mean Reciprocal Rank)** for recommendation ranking efficiency.
- **Coverage and Diversity** to evaluate recommendation variety.

## **Datasets**
@ TODO

## **References**
1. [arXiv:2310.09233](https://arxiv.org/abs/2310.09233) - Autonomous Interaction for Agent CF.
2. [arXiv:2312.10997](https://arxiv.org/pdf/2312.10997) - Retrieval-Augmented Generation (RAG).
3. [arXiv:2207.12515](https://arxiv.org/pdf/2207.12515) - Generative Search with SLMs.