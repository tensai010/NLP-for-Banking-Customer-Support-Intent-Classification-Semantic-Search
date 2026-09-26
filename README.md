# NLP-for-Banking-Customer-Support-Intent-Classification-Semantic-Search
Banking support NLP project comparing TF-IDF and sentence embeddings for intent classification and semantic search.

Business Problem

→ Classify incoming banking support tickets into 77 predefined intents

Dataset

→ BANKING77
→ 10,003 training tickets
→ 3,080 test tickets
→ 77 intent categories

Model 1

→ TF-IDF
→ Unigrams + bigrams
→ Logistic Regression
→ Accuracy: 85.8%

Error Analysis

→ virtual_card_not_working
→ Precision: 1.00
→ Recall: 0.38
→ F1: 0.55

Model 2

→ all-MiniLM-L6-v2 sentence embeddings
→ Logistic Regression
→ Accuracy: 90.81%

Key Improvement

virtual_card_not_working:
F1 0.55 → 0.89
Recall 0.38 → 0.80

Conclusion

→ TF-IDF remains strong for lexical distinctions
→ embeddings perform better where semantic context separates overlapping intents
→ model selection should be driven by error patterns, not accuracy alone

Semantic Retrieval

Historical tickets: 10,003
Test queries: 3,080

Top-1 retrieval accuracy: 92.05%
Hit@5: 97.01%
