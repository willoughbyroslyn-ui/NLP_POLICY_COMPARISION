# NLP_POLICY_COMPARISION
NLP comparison of U.S. and EU approaches to AI policy across 16 documents (8 U.S., 8 EU), each a summary of about 250 words of a major AI law, executive order, or regulation. TF-IDF divergence, topic modeling, concept dictionaries, and tone lexicons show a measurable split: EU texts use fundamental-rights terms 2.9× as often as U.S. texts, while U.S. texts use infrastructure terms 4.8× as often.

## Key results

| Measure (per 1,000 tokens) | U.S. | EU | Ratio |
| --- | --- | --- | --- |
| Fundamental rights terms | 19.0 | 55.3 | EU 2.9× |
| Rights-based tone | 19.9 | 45.4 | EU 2.3× |
| Enforcement and penalties terms | 12.4 | 45.4 | EU 3.7× |
| Transparency terms | 5.8 | 26.5 | EU 4.6× |
| Infrastructure terms | 54.6 | 11.4 | U.S. 4.8× |
| Innovation and competition terms | 64.6 | 8.3 | U.S. 7.8× |
| Permissive tone | 49.7 | 15.1 | U.S. 3.3× |

Average cosine similarity between U.S. and EU documents is 0.033, compared with 0.068 among U.S. documents and 0.078 among EU documents.

## Notes
- The corpus uses short summaries of each policy rather than full legal texts, so results describe how these policies are framed, not their complete wording.
- Results come from running `ai_policy_nlp.ipynb` as written (LDA `random_state=42`).
