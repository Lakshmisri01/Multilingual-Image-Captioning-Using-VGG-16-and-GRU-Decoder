# Multilingual-Image-Captioning-Using-VGG-16-and-GRU-Decoder
This project develops a multilingual image captioning system that supports English, Hindi, and Malayalam, aiming to enhance the inclusivity and accessibility of AI-driven technologies. It employs a specialized Transformer model for multilingual language processing in conjunction with the VGG16 architecture for robust visual feature extraction. The system improves the searchability of images by generating precise, contextually appropriate captions that enhance the metadata associated with visual content. This not only facilitates easier access to information in native languages but also aids in the preservation of linguistic heritage. 

## Dataset 
The dataset comprises 8,000 images sourced from Flickr, emphasizing everyday scenarios featuring people and animals. Each image is accompanied by five unique captions, crafted by human annotators. This rich annotation makes the dataset highly suitable for training and evaluating image captioning systems. The data is organized into predefined splits for training, validation, and testing, facilitating systematic development and assessment. Such a structure is instrumental in fostering the creation of models capable of generating realistic and contextually accurate captions.

![image](https://github.com/Lakshmisri01/Multilingual-Image-Captioning-Using-VGG-16-and-GRU-Decoder/assets/114591852/71fc997c-b4b6-4fb9-bb1f-1463d06e2883)

### captions :  
1. several climbers in a row are climbing the rock while the man in red watches and holds the line.
2. seven climbers are ascending a rock face whilst another man stands holding the rope.
3. a group of people climbing a rock while one man belays.
4. a group of people are rock climbing on a rock climbing wall.
5. a collage of one person climbing a cliff.

## Methodology

### Image Feature Extraction with VGG16
The methodology begins with the VGG16 architecture, a deep convolutional neural network originally designed for image classification tasks but adept at feature extraction. Followed by a pre-trained VGG16 model on the ImageNet dataset to process input images. This model extracts dense feature vectors that encapsulate the essential visual information of each image, providing a robust foundation for subsequent caption generation.

### Caption Generation with Transformer Model
Following feature extraction, the Transformer model takes over to handle the caption generation. This model is distinguished by its self-attention mechanism, allowing it to process data inputs in parallel, significantly enhancing efficiency compared to traditional sequential models. The Transformer architecture comprises:
- **Encoder**: Receives the image feature vectors from VGG16 and uses self-attention to interpret these features, creating a contextually enriched representation.
- **Decoder**: Generates the captions by predicting one word at a time. It employs multi-head attention to focus on various parts of the image features and previously generated words, optimizing the prediction of the next word in the sequence.

## Results 

### English
![image](https://github.com/Lakshmisri01/Multilingual-Image-Captioning-Using-VGG-16-and-GRU-Decoder/assets/114591852/a2ac5121-edf3-4cbc-bb95-b8453eb8e1f0)

### Hindi 
![image](https://github.com/Lakshmisri01/Multilingual-Image-Captioning-Using-VGG-16-and-GRU-Decoder/assets/114591852/4d1b8ffd-7ece-4388-a553-88c14abfd809)

### Malayalam 
![image](https://github.com/Lakshmisri01/Multilingual-Image-Captioning-Using-VGG-16-and-GRU-Decoder/assets/114591852/08e56479-1c37-4e1a-8b29-9803b18b9e0c)


