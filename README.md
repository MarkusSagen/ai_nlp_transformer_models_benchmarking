# Benchmarking of Transformer based NLP models
Investigates what impacts the GPU allocation, inference and training time for different Transformer based models, sequence lenghts, batch sizes, and model configurations.

This repo contains code both to:
- Benchmark new models   
- Plot the results from the benchmarks   
- Fit a linear regression model to the results and estimate the optimal regressors.  

# Run new benchmarks        
         
    poetry install
    poetry run python run_benchmarks.py
  
Edit the file to add new models, sequences or batch sizes, etc.

# The Notebook

    pip install plotly pandas numpy matplotlib nbformat dash jupyter
    cd ai_nlp_transformer_models_benchmarking/notebooks
    jupyter notebook
    
# More Info
**This notebook investigates how**:
1. Inference GPU allocation  
2. Training GPU allocation   
3. Inference time    
4. Training time  

**Changes when varying the**:   
1. sequence length   
2. batch size   
3. transformer model and size   
4. If the model is set to use half precision or not (fp16)

<b style="color: purple;">For the following Models</b>:
1. BERT_base
2. BERT_large
3. RoBERTa_base
4. RoBERTa_large
5. dist_bert
6. MiniLM
7. MiniLM_multilingual
8. mBERT_cased
9. XLM-R_base
10. XLM-R_large
11. GPT-2
12. BART_large 
13. mBART_large
14. Longformer_base
15. Longformer_large
16. BigBird
17. Transformer_XL
18. Reformer

*Models tried that did not work with the benchmark framework*:   
1. T5
2. mT5
3. wT5
4. convBERt
5. Funnel Transformer (efficient)
6. GPT-Neo
<br>
