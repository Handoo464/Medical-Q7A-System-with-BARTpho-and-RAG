**Model Performance Evaluation**  

To evaluate the accuracy of the model's predicted answers, we used the ROUGE and BLEU metrics. Below is a summary of the evaluation process:  

1. **Initialization of ROUGE and BLEU metrics**: The metrics "RougeScorer" and "SentenceBleu" were used to calculate ROUGE scores (ROUGE-1, ROUGE-2, ROUGE-L) and BLEU scores.  
2. **Iterating through questions and contexts**: The model generated answers, and the ROUGE-1, ROUGE-2, ROUGE-L, and BLEU scores were calculated for each sample.  
3. **Average scores**: The mean ROUGE-1, ROUGE-2, ROUGE-L, and BLEU scores were computed across all samples.  

**Metrics and Results:**  

| **Metric**  | **Score** | **Meaning**                                                                                  |  
|--------------|-----------|---------------------------------------------------------------------------------------------|  
| **ROUGE-1** | 0.7786    | Measures the overlap of individual words between the predicted and reference answers (77.86%).|  
| **ROUGE-2** | 0.7385    | Measures the overlap of consecutive word pairs (bi-grams), reflecting accuracy in order (73.85%).|  
| **ROUGE-L** | 0.7618    | Based on the longest common subsequence (LCS), showing structural similarity (76.18%).       |  
| **BLEU**    | 0.6565    | Evaluates the semantic accuracy using n-grams, reflecting naturalness and precision (65.65%).|  
