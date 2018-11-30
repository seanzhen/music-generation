# Style-music-generation

A cute multi-layer LSTM network that can perform like a human 🎶 It learns the dynamics of music! The architecture was specifically designed to handle music of different genres.

I just re-implemented the author's work, then please read his [blog post](http://imanmalik.com/cs/2017/06/05/neural-style.html) and paper:

> **Iman Malik, Carl Henrik Ek, [*"Neural Translation of Musical Style"*](https://arxiv.org/abs/1708.03535), 2017.**


## 准备工作

所需要的环境：python 2.7 & Tensorflow

python package

1. midi2audio
2. mido
3. pretty_midi
这三个都很容易安装

## 运行

请运行music.ipynb文件，这是我测试运行成功的文件

## The Piano Dataset
I created my own dataset for the model. If you wish to use the Piano Dataset 🎹 for academic purposes, you can download it from [here.](http://imanmalik.com/assets/dataset/TPD.zip) The Piano Dataset is distributed with a [CC-BY 4.0 license](https://creativecommons.org/licenses/by/4.0/). If you use this dataset, please reference this [paper](https://arxiv.org/abs/1708.03535):

## 文件(音乐文件太大了就自己下好了不放上来了)
`\run` : 保存了运行结果.

`\data` : 包括inputs和velocities, 最初的对音乐文件的存储.

`\predict` : 结果文件，origin是测试音频, original_classical和original_jazz都是生成的不同风格的音乐.

`main.py` : the main file to implemented.
`convert-format.rb` : This was used to convert format 1 MIDIs into format 0.  
`file_util.py` : This contains folder/file-handling functions.  
`midi_util.py` : This contains MIDI-handling functions.  
`model.py` : StyleNet's Class.  
`data_util.py` : For shuffling and batching data during training.  

