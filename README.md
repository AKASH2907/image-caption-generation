# image-caption-generation
Using FlickR8K images and text data to generate an Image Captioning System

## Dataset 
1) Flickr8k_Dataset.zip (1 Gigabyte) Contains all photographs.
2) Flickr8k_text.zip (2.2 Megabytes) Text descriptions for all photographs.

Dataset is divided into train/val/test as 6k/1k/1k images. There are total around 8k images.

## Dataset Geneation
1) Images - generate_image_features.py - VGG 16 model features
2) Text   - text_data_generation.py - LOad Clean Descriptions


## Model Summary

![model_caption](https://user-images.githubusercontent.com/22872200/43551973-92bdc306-9606-11e8-978e-4610ffcb1cbf.png)

## References
[1] [Framing Image Description as a Ranking Task: Data, Models and Evaluation Metrics](https://jair.org/index.php/jair/article/view/10833/25854)

[2] [VGG Model- Very Deep Convolutional Network](http://www.robots.ox.ac.uk/~vgg/research/very_deep/)

[3] [Where to Put the Image in Image Caption Generator](https://arxiv.org/pdf/1703.09137.pdf)
