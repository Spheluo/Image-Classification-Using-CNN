# Image-Classification-Using-CNN
Implementation of Image Classification with Convolutional Neural Network

The cifar-10 training and testing dataset and also annotation can be downloaded via the [link](https://drive.google.com/file/d/1w9Vezb2rSbEMfl_IHzR0Hfeyi7c_JQKf/view?usp=sharing).

## Strategy:
We will train three different kinds of CNN models (myLeNet, myResNet, and built-in ResNet18) and plot learning curves to evaluate the accuracies and losses of an individual epoch. For each CNN model, the epoch with the best accuracy on validation sets will be preserved as pt files for the assessment of testing data. The performance reached a strong baseline when using pre-trained ResNet18 and data augmentation by 'RandomHorizontalFlip'.

## Steps:

### 1. Use the following script to train the model 'myLeNet':
python3 main.py --model 'LeNet'
### 2. Use the following script to test the model:
python3 eval.py --path 'save_dir/LeNet/best_model.pt' --model 'LeNet'

### 3. Use the following script to train the model 'myResNet':
python3 main.py --model 'ResNet'
### 4. Use the following script to test the model:
python3 eval.py --path 'save_dir/ResNet/best_model.pt' --model 'ResNet'

### 5. Use the following script to train the pytorch built-in model 'ResNet18':
python3 main.py --model 'ResNet_18’
### 6. Use the following script to test the model:
python3 eval.py --path 'save_dir/ResNet_18/best_model.pt' --model 'ResNet_18'

## Accuracy Results:
myLeNet acc=0.57 | myResNet acc=0.77 | Resnet18 acc=0.8034.
