# Network Traffic Classification using DAE-BYOL



## Full report  (bit in progress)
https://docs.google.com/document/d/1UfTX9nY3h6HOpv-4OhZPO9AIa3x7MXwarfY1n4oaAeU/edit?usp=sharing

## What this is
A class project testing whether combining denoising autoencoders with BYOL works for botnet detection. Got decent results on CTU-13 dataset.

## The approach
1. Train a denoising autoencoder on noisy network features
2. Use the DAE encoder in a BYOL framework (in the online and target notwork)
3. Classify the learned embeddings with Random Forest

## Results
- 93% accuracy on test set
- AUROC: 0.98
- Embeddings show clear separation between normal/botnet traffic

