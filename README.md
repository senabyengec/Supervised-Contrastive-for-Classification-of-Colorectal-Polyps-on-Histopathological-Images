# Supervised-Contrastive-for-Classification-of-Colorectal-Polyps-on-Histopathological-Images

### Overview
This notebook presents an implementation of the "An Effective Colorectal Polyp Classification for Histopathological Images" article. Our focus is on constructing a Supervised Contrastive Learning (Sup-Con) model, specifically designed for classifying colorectal polyps in colon histopathology images.

### Model Architecture
The proposed model enhances the standard Sup-Con framework with several architectural modifications. Key among these is the integration of the Big Transfer (BiT) encoder. We further refine the model in a second stage by introducing an intricate sequence of layers, including dropout layers and a fully connected layer equipped with L2 kernel regularizers. The architecture culminates in a softmax layer for final classification.

### Optimization and Loss Function
For optimization, we employ Stochastic Gradient Descent (SGD), carefully calibrated with an optimal learning rate and momentum. The model's robustness and accuracy are further boosted by our choice of loss function: categorical cross-entropy with label smoothing. This choice not only enhances prediction accuracy but also improves the model's adaptability in various scenarios.

**Author of the code: Sena Yengec-Tasdemir**

## Requirements
*   The dataset need to be uploaded to Google Drive folder. The following paths need to be updated accordingly.
*   Wandb is used for plots. One needs to either have a Wandb account or remove those lines of code.
