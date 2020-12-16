### Jetson Nano DeepSpeech in Spanish and English


* Install Dependencies
```
pip install deepspeech-0.9.0-cp36-cp36m-linux_aarch64.whl
```

* List Devices
Found your device and check the simple rate
use:
```
python3 list_devices.py 
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
