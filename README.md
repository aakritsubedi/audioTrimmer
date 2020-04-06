# Audio Trimmer using pydub

### Install FFmpeg
Install FFmpeg for your OS following the instruction given below:  
 - (https://github.com/adaptlearning/adapt_authoring/wiki/Installing-FFmpeg)[https://github.com/adaptlearning/adapt_authoring/wiki/Installing-FFmpeg]
  - **Ubuntu**
    - sudo add-apt-repository ppa:mc3man/trusty-media  
    - sudo apt-get update  
    - sudo apt-get install ffmpeg  
    - sudo apt-get install frei0r-plugins  

After that you need to add the libary to your system path for python to be able to find and to use it. That can be done by either actually adding the installation path of FFmpeg to your OS path (How to do that depends on your operating system), or by adding it to the temporary path variable that is used inside of python.
  - `import sys`
  - `sys.path.append('/path/to/ffmpeg')` 
  Eg. `sys.path.append('/usr/bin/ffmpeg')`

### Create a virtualenv 
  - `virtualenv venv -p python3.6`

### Activate the virtual environment
  - `source venv/bin/activate`

### Install necessary packages
  - `pip3 install -r requirements.txt`

### Run `audio_trimmer.py` file
  -  `python3`
  - `from audio_trimmer import  *`
  - `audioTrimmer('let',0,00,0,30)`

### Output
  - Inside `mp3` folder `let-extract.mp3`
