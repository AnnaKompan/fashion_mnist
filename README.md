# FASHION MNIST

## Model can be used to make predictions of:

1. T-shirt/top
2. Trouser
3. Pullover
4. Dress
5. Coat
6. Sandal
7. Shirt
8. Sneaker
9. Bag
10. Ankle boot

## Requied Python Packages

`pip install torch torchvision matplotlib`

## Training Setup

- **CrossEntropy loss function** - for multi-class classification (10 classes)
- **Adam optimizer** - adapts learning rate per parameter, faster convergence compared to SGD
- Transformations:
  **ToTensor** - values scaled from 0,250 to 0.0, 1.0
  **Normalize** - substracted mean 0.5 and divided by std 0.5 -> px range -1, 1
- Model

## Training Results (20 epochs)

- **Average loss is 0.8** - model fits training data well
- **Test accuracy is 88.9%** - means generalization on test data

- Higher average train loss compared to test loss means model overfits
  -> data augmentation and regularization would fix this problem

[Train Results]('./train_result.png')

[Prediction results]('./prediction.png')

## Training loss per epoch

Training loss steadily decreasing
[Train Loss]('./train_loss.png')
