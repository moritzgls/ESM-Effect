



### ESM-Effect: An Effective and Efficient Fine-Tuning Framework Towards Accurate Prediction of Mutation's Functional Effect

Code accompanying the [pre-print](https://www.biorxiv.org/content/10.1101/2025.02.03.635741v1) *"ESM-Effect: An Effective and Efficient Fine-Tuning Framework Towards Accurate Prediction of Mutation's Functional Effect"*.


Train and test ESM-Effect to predict the functional effect of missense mutations from a Deep Mutational Scan (DMS).

The notebook contains:
- Data preprocessing
- An experiment manager to create new experiments with different setups and evaluations
- Logging in TensorBoard
- Training, testing, and plotting predictions according to the proposed benchmarking framework

Key Features:
- Full & optimized ESM-Effect implementation
- **ESM-Effect Speed**: Caching embeddings from the 10th layer during the first epoch, and forward-passing & training only the last two layers in the remaining epochs. This results in an 8.4x speedup over the optimized ESM-Effect and a 56.3x speedup over the state-of-the-art method *PreMode*, with slightly better performance.
