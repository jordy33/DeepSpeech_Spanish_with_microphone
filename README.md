### Jetson Nano DeepSpeech in Spanish and English

![](gif/DeepSpeech.gif)

* git clone this repository and then
```
cd ~
git clone https://github.com/jordy33/Jetson-Nano-DeepSpeech-in-Spanish-microphone.git
cd Jetson-Nano-DeepSpeech-in-Spanish-microphone 
```
* Install Dependencies
```
pip install deepspeech-0.9.0-cp36-cp36m-linux_aarch64.whl
```

* Uncompress Spanish model
```
cd models/es
cat x* > spanish_model.tar.gz
tar -vxf spanish_model.tar.gz
cd ../../
```
* Uncompress English model 0.9.0 in ~/models/en
Download deepspeech-0.9.0-models.pbmm and deepspeech-0.9.0-models.scorer
from [here](https://github.com/mozilla/DeepSpeech/releases)

* Execute translation
Will ask for device, sample rate of the device and the language (pick spanish)
use:
```
python3 mic_vad_streaming.py 
```

