# image-caption-generation
Using FlickR8K images and text data to generate an Image Captioning System

## Dataset 
1) Flickr8k_Dataset.zip (1 Gigabyte) Contains all photographs.
2) Flickr8k_text.zip (2.2 Megabytes) Text descriptions for all photographs.

Dataset is divided into train/val/test as 6k/1k/1k images. There are total around 8k images.

## Dataset Geneation
1) Images - generate_image_features.py - VGG 16 model features
2) Text   - text_data_generation.py - Load Clean Descriptions

The function below named create_sequences(), given the tokenizer, a maximum sequence length, and the dictionary of all descriptions and photos, will transform the data into input-output pairs of data for training the model. There are two input arrays to the model: one for photo features and one for the encoded text. There is one output for the model which is the encoded next word in the text sequence.

## Model Summary

![Model Summary](https://user-images.githubusercontent.com/22872200/43551973-92bdc306-9606-11e8-978e-4610ffcb1cbf.png)

## References
[1] [Framing Image Description as a Ranking Task: Data, Models and Evaluation Metrics](https://jair.org/index.php/jair/article/view/10833/25854)

[2] [VGG Model- Very Deep Convolutional Network](http://www.robots.ox.ac.uk/~vgg/research/very_deep/)

[3] [Where to Put the Image in Image Caption Generator](https://arxiv.org/pdf/1703.09137.pdf)
[4] [BLEU Score Metrics](http://www.nltk.org/api/nltk.translate.html)

