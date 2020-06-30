# iris

## Development Notes
1. `python3 -m venv env`
2. `source env/bin/activate`

## Dependency issues
1. `pip install SpeechRecognition` (after confirming python3.6.9 for both python3 and pip)
2. `pip install pyaudio`
3. `pip install wheel` (because "invalid command `bdist_wheel`") (https://github.com/tensorflow/tensorflow/issues/348)
4. Try #2 again.
5. "Python.h: No such file or directory"
6. `sudo apt-get install libpython3.6-dev`
7. Try #2 again.
8. "Failed building wheel for pyaudio. Fatal error: portaudio.h: No such file or directory"
9. `sudo apt-get install portaudio19-dev python-pyaudio python3-pyaudio` (https://stackoverflow.com/questions/48690984/portaudio-h-no-such-file-or-directory)
10. Try #2 again. Success!
11. Try running `python -m speech_recognition`. It fails, because it can't find my mic. Cry.
