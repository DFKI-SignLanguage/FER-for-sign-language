# Facial expression recognition for Sign Language

## Introduction 

With this code we investigate the capability of convolutional neural networks to recognize in sign language video frames the six basic Ekman facial expressions for ‘fear’, ‘disgust’, ‘surprise’, ‘sadness’, ‘happiness’, ‘anger’ along with the ‘neutral’ class. Given the limited amount of annotated facial expression data for the sign language domain, we started from a model pre-trained on general-purpose facial expression datasets and we applied various machine learning techniques such as fine-tuning, data augmentation, class balancing, as well as image preprocessing to reach a better accuracy. The models were evaluated using K-fold cross-validation to get more accurate conclusions. It is experimentally demonstrated that fine-tuning a pre-trained model along with data augmentation by horizontally flipping images and image normalization, helps in providing the best accuracy on the sign language dataset. The best setting achieves satisfactory classification accuracy, comparable to state-of-the-art systems in generic facial expression recognition. Experiments were performed using different combinations of the above-mentioned techniques based on two different architectures, namely MobileNet and EfficientNet, and is deemed that both architectures seem equally suitable for the purpose of fine-tuning, whereas class balancing is discouraged.

## Reference

This code is associated with the SLTAT2022 publication: https://aclanthology.org/2022.sltat-1.5/

```
@inproceedings{deshpande-etal-2022-fine,
    title = "Fine-tuning of Convolutional Neural Networks for the Recognition of Facial Expressions in Sign Language Video Samples",
    author = "Deshpande, Neha  and
      Nunnari, Fabrizio  and
      Avramidis, Eleftherios",
    booktitle = "Proceedings of the 7th International Workshop on Sign Language Translation and Avatar Technology: The Junction of the Visual and the Textual: Challenges and Perspectives",
    month = jun,
    year = "2022",
    address = "Marseille, France",
    publisher = "European Language Resources Association",
    url = "https://aclanthology.org/2022.sltat-1.5",
    pages = "29--38",
}

```

The code is an extension of the code provided by 
https://github.com/HSE-asavchenko/face-emotion-recognition
