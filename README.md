# Apparel-classification-webapp-using-CNN

In this repo , I'll use mnist clothing images to classify different Appreals.
This system can diffrentiate 9 types of clothings namely "Tshirt","Trouser","Pullover","Dress","Coat","Sandal","Shirt","Sneaker","Bag","Ankle boot" . 


## **Preprocessing**

The images are of varying length and width and are all resized,normalized the pixels and change color profile to grayscale, segementation all so proves to be useful for the model in simplifying the image.

## **Training**

For Training I've used 2 Conv layers followed by a MaxPooling layer with batch normalizing after conv layers, i used drop out of 0.25 after Maxpooling and 0.5 after dense layer.I used Relu activation function for 2Conv and Dense Layers. I've trained the model for 100 epochs.

## **Evaluation**

The model's performance is evaluated on test data and we used accuracy for evaluation.The test accuracy was 0.93.

## **Deployment**

The deployment is very basic and I've used Flask for it. Save the model weights in 'models' ,run the app.py file and go to http://localhost:5000. Upload the Apparel image of your choice and give it to the model to predict it
