# Remote-sensing-image-retrieval-deep-learning-
Enhanced remote sensing image retrieval using deep learning techniques

This repository contains experiments on content-based remote sensing image retrieval (RSIR) using multiple deep convolutional neural network (CNN) architectures and their fusion. The models were evaluated on two benchmark datasets: UC Merced and PatternNet.

📌 Models Used

We experimented with several CNN architectures:

ResNet family: ResNet50, ResNet101, ResNet152

VGG family: VGG16, VGG19

MobileNet

InceptionV3

⚡ Approach
🔹 Single CNN Evaluation

Each model was tested individually for retrieval performance.

MobileNet achieved the best single-model performance:

UC Merced: MAP = 65.32%

PatternNet: MAP = 71.99%

VGG models showed the weakest results, with higher ANMRR values.

🔹 Pairwise Model Fusion

Feature vectors from two CNNs were fused to enhance representation.

Best result on PatternNet: ResNet50 + ResNet152 → 83.01% MAP

Best result on UC Merced: ResNet50 + ResNet101 → 71.27% MAP

🔹 Full Model Family Fusion

Combining multiple models from the same family further improved retrieval.

ResNet50 + ResNet101 + ResNet152 achieved the best overall performance:

UC Merced: MAP = 77.44%, ANMRR = 0.0252

PatternNet: MAP = 82.92%, ANMRR = 0.0128

📊 Key Findings

MobileNet was the strongest single model, thanks to its lightweight yet effective feature extraction.

Pairwise fusion of ResNets significantly improved retrieval accuracy compared to individual models.

Full ResNet family fusion achieved the best overall performance, showing the advantage of combining multi-depth feature hierarchies.

🛠️ Tech Stack

Languages & Frameworks: Python, TensorFlow / PyTorch

Datasets: UC Merced, PatternNet

🚀 Results Summary

Single models ranking: MobileNet > ResNet > InceptionV3 > VGG

Fusion models ranking: ResNet family fusion > Pairwise ResNet fusion > MobileNet fusion

Best configuration: ResNet50 + ResNet101 + ResNet152



📄 Research Paper  
This work is part of an ongoing research study.  
The research paper based on these experiments is currently **under preparation / review** and will be uploaded here once officially published.  
