# NLP

* Avoid spelling mistakes using beam search, dictionary and language model with bigrams and unigrams

# Included Models

------------------------------


Architecure | Embeddings | Done | WER | Inference Time
------------ | ------------- |----------|-------|--------|
Marbert (Seq) | 100k Word| :heavy_check_mark: | 0.14 | 3.12 sec / word
LM (BI & UNI) | Bi-gram & Uni-gram| :heavy_check_mark: | 0.10667 | 5.72 µs / word 
Marbert (batch) | 100k Word| :heavy_multiplication_x: | -- | ---
Marbert (batch) | 670k Word| :heavy_multiplication_x: | -- | ---


# Pipeline
The Encoded Sentence is fed into the algorithm. Inputs enables word beam search decoding Fucntion to create a dictionary and LM. Different settings control how the LM scores the beams (text candidates) and how many beams are kept per time-step. The algorithm outputs the decoded text. The following illustration shows the pipeline. <br/>
![Pipeline](pipeline/xx.png)



