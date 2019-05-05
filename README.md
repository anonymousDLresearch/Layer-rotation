## Layer rotation: a surprisingly simple indicator of generalization in deep learning?

Code to reproduce results of paper "Layer rotation: a surprisingly simple indicator of generalization in deep networks?"

### Code structure
Code structure tries to follow the structure of the paper. Name of folders correspond to the name of sections of the paper.

*experiment_utils* provides basic utilities useful for data management and training of deep networks

*get_training_utils* provides training parameters such as (optimized) learning rate schedules for each of the 5 tasks

*import_task.py* and *models.py* are used to load the data and the untrained models corresponding to the 5 tasks used in the experiments.

*layer_rotation_utils.py* contains the code for creating layer rotation curve visualizations

*layca_optimizers.py* contains the code to apply Layca on SGD, Adam, RMSprop or Adagrad, and to use layer-wise learning rate multipliers when using SGD (cfr. alpha parameter).

### Libraries configuration
Code was run with tensorflow-gpu 1.8.0 and keras 2.2.4
