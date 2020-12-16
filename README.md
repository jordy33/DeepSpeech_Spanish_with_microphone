### Jetson Nano DeepSpeech in Spanish and English

![](gif/DeepSpeech.gif)

* Software Requirements for the Jetson Nano: The last Jetson Nano SD Card Image

* Hardware Requirements for the Jetson Nano: USB audio card and microphone 

* git clone this repository 
```
cd ~
git clone https://github.com/jordy33/Jetson-Nano-DeepSpeech-in-Spanish-microphone.git
cd Jetson-Nano-DeepSpeech-in-Spanish-microphone 
```
* Install Dependencies
* Download the file  deepspeech-0.9.0-cp36-cp36m-linux_aarch64.whl from [here](https://github.com/domcross/DeepSpeech-for-Jetson-Nano/releases) and execute the following command
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

* If you also want the translation in english Download deepspeech-0.9.0-models.pbmm and deepspeech-0.9.0-models.scorer from [here](https://github.com/mozilla/DeepSpeech/releases) in the directory ~/models/en otherwise skip this step

* Execute translation
Will ask for device, sample rate of the device and the language (pick spanish)
use:
```
python3 mic_vad_streaming.py 
```

