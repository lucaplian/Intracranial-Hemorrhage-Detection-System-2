# Second-stage for Intracranial Hemorrhage Detection System

Homework within the course of Supervised Learning. In this stage, we had to explore using k-fold validation and used diverse techniques to improve the accuracy of the model when using the test dataset. A short clarification beforehand: the model we are using is multilabel, and the accuracy used is subset accuracy (meaning that all labels must match each other). The project is divided into 7 parts:
* Part 1: We explored the accuracy of each fold without using any finetuning
* Part 2: We delved into adding weight, oversampling and augmentation for one particular fold
* Part 3: We examined the three transformations in depth: normal transformations, moderate augmentation and aggressive augmentation, done for all five folds
* Part 4: We analysed the usage of Early Stop and LR Scheduler - StepLR and Plateau
* Part 5: We conducted an ablation study to explore diverse techniques. We found out that Dropout(p=0.3), FocalLoss(alpha=0.5, gamma=2), and ReduceLRPlateau(f=0.1, patience=3), provided the best results in the accuracy department
* Part 6 (Bonus 2): We had to explore the quantitative metrics of the model using the previous techniques, which proved the best were Dropout, FocalLoss, and ReduceLRPlateau. We tested them using a pretrained model for two scenarios: with the backbone frozen and unfrozen. The unfrozen model achieved 48% accuracy, which is good for an unbalanced dataset and a strict accuracy metric.
* Part 7 (Bonus 1): We had to perform a qualitative analysis, including GradCAM, on correctly and incorrectly predicted images. Project structure:
* part_1234.ipynb - it dealt with the first four parts
* part_5.ipynb - it dealt with part 5
* part_5-continuation.ipynb - it continued the part done in part 5, but we added other metrics, which were unconsidered in part_5
* part_6(bonus 2).ipynb - it dealt with part 6
* part_7(bonus 1).ipynb - it dealt with part 7
* luca_plian_raport_etapa2_inv_sup.pdf - it is the report, which was done as part of this project
