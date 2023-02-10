# GreenNets: Energy Efficient Deep Learning Models
Maximizing Accuracy and Energy & CO2 Consumption

Drexel AI 2023 Winter Project

## Introduction:

## Background
https://arxiv.org/abs/1910.09700
https://arxiv.org/abs/2007.03051
https://dl.acm.org/doi/abs/10.5555/3455716.3455964
https://arxiv.org/abs/2104.10350
https://arxiv.org/pdf/2203.02202.pdf

## Methods

### Carbon Tracker:
* https://github.com/lfwa/carbontracker

```
from carbontracker.tracker import CarbonTracker

tracker = CarbonTracker(epochs=max_epochs)

# Training loop.
tracker.epoch_start()
    
# Your model training.
model.train(X_train, y_train)

tracker.epoch_end()

# Optional: Add a stop in case of early termination before all monitor_epochs has
# been monitored to ensure that actual consumption is reported.
tracker.stop()
```

### Models: (Alisha, Alex, Yashodha)
*   ResNet
*   VGG
*   EfficientNet
*   MobileNetV2

### Datasets:
In order from largest to smallest
*   ImageNet - Alex
*   CIFAR-10 - Alisha
*   MNIST - Yashodha

For each dataset:
* Train each model on the dataset & measure Energy (kWh) & Co2eq consumption (g) for 20-100 epochs to get to 80% accuracy
    * retrain model using different batch sizes in [4,8,16,32,64,128,256,450] and a different number of epochs (consistent accross the samples)
    * measure accuracy, energy, and co2 consumption
