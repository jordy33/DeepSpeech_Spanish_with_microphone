### Jetson Nano DeepSpeech in Spanish and English


* Install Dependencies
```
pip install deepspeech-0.9.0-cp36-cp36m-linux_aarch64.whl
```

* Uncompress model
* git clone this repository and then
```
cd models
cd es
cat x* > spanish_model.tar.gz
tar -vxf spanish_model.tar.gz
cd ../../
```

* Execute translation
Will ask for device, sample rate of the device and the language (pick spanish)
use:
```
python3 mic_vad_streaming.py 
```

Get the device id by example: my usb card is called pulse adjust the code with your usb card name

Update eng.sh and esp.sh with the device number and sampling rate

To start translation from Microphone voice in spanish to text run:

```
./esp.sh
```

To start translation from Microphone voice in english to text run:
```
./eng.sh
```
