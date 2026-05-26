# TML-Model-Stealing
Our approach compares the functional behaviour of each suspect model against the target model by
running both on the same fixed set of inputs (the CIFAR-100 test set). And measures the similarity
of their output logits. All experiments used 40 batches of 256 images (10,240 samples total). Code
is available at: https://github.com/arcnova2095/TML-Model-Stealing

# Methodology Used
KL divergence between the softmax output distributions of the target and suspect and evaluated per sample and averaged across the dataset. To obtain
a confidence score (higher = more stolen)

