# xiaolan---
这是一个中文的智能家居控制对话机器人——由叮当衍生而来，目前还未100%完成，所以发上来，希望大家一起研发，一个人研发也没那么多点子和经验
一、本机器人的测试环境为：
1、树莓派3B
2、python
3、阵列麦克风（可换）
4、海威特音响（可换）

二、使用方法：
1、准备以上硬件
2、将小蓝git下来
3、安装一下东东：
  sudo apt-get install cmake g++ gcc
  sudo apt-get install python2.7 python3 python-pyaudio python3-pyaudio sox
  su root(如果还没有启用root账户，输入sudo passwd root, sudo passwd --unlock root)
  pip install pyaudio
  sudo apt-get install python3-dev python-dev libatlas-base-dev
3、修改/测试(可以在github修改了再提交

三、文件体系：
xiaolan:
  - xldo.py #中心文件
  - stt.py #语音转文字
  - tts.py #文字转语音
  - speaker.py #音响
  - recorder.py #录音
  - snowboy.py #snowboy主控
  - musiclib #音乐库
    - ding.wav
    - dong.wav
    - welcome.mp3
  - snowboy #snowboy唤醒引擎
    - demo.py
    - snowboydecoder.py #snowboy主要文件
    - xiaolanxiaolan.pmdl #小蓝小蓝唤醒词
    - .....(不一一列举）
  
