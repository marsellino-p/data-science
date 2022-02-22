# Fruit Classification using Transfer Learning InceptionV3 

This repository is about Deep Learning to classify types of fruits and vegetables.

Dataset used in this repository is retrieved from [Kaggle](https://www.kaggle.com/moltean/fruits)

Here are the dataset descriptions:

The following fruits and are included:
Apples (different varieties: Crimson Snow, Golden, Golden-Red, Granny Smith, Pink Lady, Red, Red Delicious), Apricot, Avocado, Avocado ripe, Banana (Yellow, Red, Lady Finger), Beetroot Red, Blueberry, Cactus fruit, Cantaloupe (2 varieties), Carambula, Cauliflower, Cherry (different varieties, Rainier), Cherry Wax (Yellow, Red, Black), Chestnut, Clementine, Cocos, Corn (with husk), Cucumber (ripened), Dates, Eggplant, Fig, Ginger Root, Granadilla, Grape (Blue, Pink, White (different varieties)), Grapefruit (Pink, White), Guava, Hazelnut, Huckleberry, Kiwi, Kaki, Kohlrabi, Kumsquats, Lemon (normal, Meyer), Lime, Lychee, Mandarine, Mango (Green, Red), Mangostan, Maracuja, Melon Piel de Sapo, Mulberry, Nectarine (Regular, Flat), Nut (Forest, Pecan), Onion (Red, White), Orange, Papaya, Passion fruit, Peach (different varieties), Pepino, Pear (different varieties, Abate, Forelle, Kaiser, Monster, Red, Stone, Williams), Pepper (Red, Green, Orange, Yellow), Physalis (normal, with Husk), Pineapple (normal, Mini), Pitahaya Red, Plum (different varieties), Pomegranate, Pomelo Sweetie, Potato (Red, Sweet, White), Quince, Rambutan, Raspberry, Redcurrant, Salak, Strawberry (normal, Wedge), Tamarillo, Tangelo, Tomato (different varieties, Maroon, Cherry Red, Yellow, not ripened, Heart), Walnut, Watermelon.

___

Dataset properties

The total number of images: 90483.

Training set size: 67692 images (one fruit or vegetable per image).

Test set size: 22688 images (one fruit or vegetable per image).

The number of classes: 131 (fruits and vegetables).

Image size: 100x100 pixels.

Filename format: imageindex100.jpg (e.g. 32100.jpg) or rimageindex100.jpg (e.g. r32100.jpg) or r2imageindex100.jpg or r3imageindex100.jpg. "r" stands for rotated fruit. "r2" means that the fruit was rotated around the 3rd axis. "100" comes from image size (100x100 pixels).

That's mean, the images from this dataset has already rotated, so in this code, we are not performing images rotation, but we have to preprocess the images its has (224, 224) of height and width for the input of the InceptionV3
___

Google's Inception V3 is the third version in a series of Deep Learning Convolutional Architectures. Inception V3 was trained with 1,000 classes from the original ImageNet dataset, which was trained with over 1 million training images. Inception V3 was trained for the ImageNet Large Visual Recognition Challenge, where it came in first place.

![inception-v3](https://camo.githubusercontent.com/d93725579fc7e7140a60faadaaf47ae93eda84b6/68747470733a2f2f7777772e50657465724d6f7373416d6c416c6c52657365617263682e636f6d2f6d656469612f696d616765732f7265706f7369746f726965732f434e4e2e6a7067)

Deep learning neural networks, such as convolutional neural networks, are a type of deep learning neural network. These sorts of neural nets are frequently employed in computer vision and have improved computer vision capabilities in recent years, performing far better than previous, more traditional neural networks; nonetheless, studies reveal that there are trade-offs related to training timeframes and accuracy.

Transfer learning allows us to retrain the final layer of an existing model, resulting in a significant reduction in both training time and dataset size. Inception V3 is one of the most well-known models that can be utilized for transfer learning. As previously said, our model was trained on over a million photos from 1,000 classes on some quite strong machines. The ability to retrain the last layer implies that we can keep the knowledge that the model gained during its original training and apply it to your smaller dataset, resulting in highly accurate classifications without the requirement for lengthy training and computer capacity. Then, in this code, we train the model with 131 classes using fully-connected layers.

(Source: [Intel](https://www.intel.com/content/www/us/en/developer/articles/technical/inception-v3-deep-convolutional-architecture-for-classifying-acute-myeloidlymphoblastic.html))
___

### Conclusion

Using Adam Optimizer, InceptionV3 achieved 97.42% of Training Accuracy and 90.02% of Validation Accuracy. You can download the constructed models on [Google Drive](https://drive.google.com/drive/folders/19i4X48dRV_oxxIXXAeZQKdU2pnwHc0T9?usp=sharing) as I couldn't upload them to Github because the models are over 100 MB each.. When we test it using random downloaded images from Google Image (in this case we are using watermelon), the model can predict it precisely. Here is the gif image of about using the model to predict the watermelon: 

![predict](https://drive.google.com/u/0/uc?id=1rC7U5az4l0K5NQrr4geR9LPkSzuj2LFi&export=download)