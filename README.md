# Vision-Skills
Code for the [Vision Skills Needed to Answer Visual uestions](https://www.ischool.utexas.edu/~dannag/publications/2020_CSCW_VQA-Skills.pdf)

## Requirements ##
- tensorflow v1.14
- keras v2.3.1 (for the pre-trained model ResNet152)

## Files ##
```./```
- ```sample_code.ipynb```: demo of skill prediction using Resnet152 feature maps.
- ```build_vocab.ipynb```: demo of how to create vocabulary for your own task.

```./csv```
- ```vizwiz_skill_typ_{test/train/val}.csv```: skill annotations for the VizWiz dataset.
- ```vqa_skill_typ_{test/train/val}.csv```: skill annotations for the selected images from the VQA2.0 dataset.

```./utils```
- ```VqaQualityModel.py```: model for vision skill prediction.
- ```word2vocab_{vizwiz/vqa}```: Ids of tokenized frequent words in the questions in the VizWiz/VQA dataset.

```./ckpt/{vizwiz/vqa}/{cnt/col/txt}```: checkpoints for the prediction of counting/color recognition/text recognition for the VizWiz/VQA dataset, respectively.


## References ##
- [VizWiz Project](http://vizwiz.org)
- [Bottom-Up and Top-Down Attention for Image Captioning and Visual Question Answering](https://arxiv.org/abs/1707.07998)
