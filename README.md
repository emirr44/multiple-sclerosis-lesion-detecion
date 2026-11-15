## Multiple Sclerosis Lesion Segmentation

Team name: FEA-MS

Project members and roles:
- **Emir Baručija**: reduction of false positive candidates
- **Farah Piralić**: segmentation of raw scans and candidate generation
- **Asja Smječanin**: data preprocessing, results evaluation

In this project, we aim to develop model capable of automatically segmenting multiple sclerosis lesions. Magnetic Resonance Imaging (MRI) scans are used as data. First we preprocess them,  removing any non-brain tissues, such as the skull and scalp, to focus our model only on brain tissue. Since training of full-scans is computationally infeasible, we crop patches around lesions. Segmentation is a two-stage process, which consists of candidates detection with nnU-Net, and false positie reduction with classification model. Main metrics include Dice score, absolute volume difference, lesion-wise precision and f1 score.
