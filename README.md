# InterviewSpeakerTranscription
Useses Openai [whsiper](https://github.com/openai/whisper) and [pyannot.audio](https://github.com/pyannote/pyannote-audio) to transcribe audio from interviews and focus groups with speaker identification.

Cite pyannot audio if you use it for a paper:

```
@inproceedings{Bredin2020,
  Title = {{pyannote.audio: neural building blocks for speaker diarization}},
  Author = {{Bredin}, Herv{\'e} and {Yin}, Ruiqing and {Coria}, Juan Manuel and {Gelly}, Gregory and {Korshunov}, Pavel and {Lavechin}, Marvin and {Fustes}, Diego and {Titeux}, Hadrien and {Bouaziz}, Wassim and {Gill}, Marie-Philippe},
  Booktitle = {ICASSP 2020, IEEE International Conference on Acoustics, Speech, and Signal Processing},
  Year = {2020},
}
```
```
@inproceedings{Bredin2021,
  Title = {{End-to-end speaker segmentation for overlap-aware resegmentation}},
  Author = {{Bredin}, Herv{\'e} and {Laurent}, Antoine},
  Booktitle = {Proc. Interspeech 2021},
  Year = {2021},
}
```
# Setup

- Create a `data` folder and put your audio files into that (current default is m4a but should work with any file format - have to change things in the ffmpeg code line).

- Run the notebook `00-TranscribeInterviewsSpeakerdetection.ipynb` - pip install missing packages

## TODO

- [ ] Make sure pyannot.audio pipeline uses GPU, as currently preprocessing takes way too long
- [ ] Add pip installs for all packages to the notebook
- [ ] Improve README
