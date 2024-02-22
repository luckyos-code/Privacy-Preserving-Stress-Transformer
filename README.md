# Abstract

We present the first privacy-preserving approach for stress detection from wrist-worn wearables based on the Time-Series Classification Transformer (TSCT) architecture and incorporating Differential Privacy (DP) to ensure provable privacy guarantees. The non-private baseline results prove the TSCT to be an effective model for the given task. Our DP experiments then show that the private models suffer from reduced utility but can still be used for reliable stress detection depending on the application. Our proposed approach has potential applications in smart health, where it can be used to monitor smartwatch users' stress levels without compromising their privacy and provide timely interventions or suggestions to prevent adverse health outcomes. Another primary contribution is our evaluation, which studies and shows negative effects of DP regarding model training. The results of this work provide perspectives for future research and applications whenever the fields of stress detection and data privacy intervene.

# Dataset

The [`WESAD-Dataset`](https://dl.acm.org/doi/10.1145/3242969.3242985) is used to train and evaluate the model.


### Setup

1. Download the dataset [here](https://ubicomp.eti.uni-siegen.de/home/datasets/icmi18/) and save the WESAD directory inside the [`data directory`](https://github.com/BDegenkolb/Privacy-Preserving-Stress-Transformer/tree/main/data).

2. To train the Transformer-model follow the notebook for the [`Transformer-model`](https://github.com/BDegenkolb/Privacy-Preserving-Stress-Transformer/blob/main/code/transformer.ipynb).
  
      Run "NeptuneAI" cell if you want to use neptuneAI, but don't forget to put your api token and project name in the "Hyperparameter" cell
  
3. Use the [`AutomatedTransformer`](https://github.com/BDegenkolb/Privacy-Preserving-Stress-Transformer/blob/main/code/AutomatedTransformer.ipynb) to train one transformer after another in a loop.
