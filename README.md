# Image-Classification-Using-CNN
Implementation of Image Classification with Convolutional Neural Network

cifar-10 training and testing dataset and also annotation can be downloaded from the [link](https://drive.google.com/file/d/1w9Vezb2rSbEMfl_IHzR0Hfeyi7c_JQKf/view?usp=sharing).

## strategy:
We will train three different kinds of CNN models (myLeNet, myResNet, and built-in ResNet18) and plot learning curves to evaluate the accuracies and losses of an individual epoch. For each CNN model, the epoch with the best accuracy on validation sets will be preserved as pt files for the assessment of testing data. The performance reached a strong baseline when using pre-trained ResNet18 and data augmentation using 'RandomHorizontalFlip'.

### 1. train and test the model myLeNet by the command:
python3 main.py --model 'LeNet'
python3 eval.py --path 'save_dir/LeNet/best_model.pt' --model 'LeNet'

### 2. train the model myResNet by the command:
python3 main.py --model 'ResNet'
python3 eval.py --path 'save_dir/ResNet/best_model.pt' --model 'ResNet'

### 3. train the pytorch built-in model 'ResNet18' by the command;
python3 main.py --model 'ResNet_18’
python3 eval.py --path 'save_dir/ResNet_18/best_model.pt' --model 'ResNet_18'
