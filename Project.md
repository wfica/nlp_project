# NN+NLP Project

### Team members
* Jakub Kuciński
* Wojciech Fica
* Jakub Dworzański

### Project title
Musical notes generation

## Description
We want to use neural networks based models to generate subsequent musical notes based on some (short) initial sequence of notes.

### Data
[Lakh Pianoroll Dataset](https://salu133445.github.io/lakh-pianoroll-dataset/?fbclid=IwAR0_N-3A5eHLrA8_HtYadnUvfOcdzugzHyiOVpUqfEqaFSRXRFSeTQiCCC8) is a collection of 174,154 multitrack pianorolls derived from the Lakh MIDI Dataset (LMD).

or maybe

[MAESTRO](https://magenta.tensorflow.org/datasets/maestro) (MIDI and Audio Edited for Synchronous TRacks and Organization) is a dataset composed of about 200 hours of virtuosic piano performances captured with fine alignment (~3 ms) between note labels and audio waveforms.

### Literature
[Deep Learning Music Generation](https://cs230.stanford.edu/projects_fall_2019/reports/26258004.pdf)

[MuseNet](https://openai.com/blog/musenet/)

[Compound Word Transformer: Learning to Compose Full-Song Music cover Dynamic Directed Hypergraphs](https://arxiv.org/pdf/2101.02402v1.pdf)

### Models
LSTM, transformers if we have enough time after it has been introduced at the lecture.

### Success evaluation
Empirical - if model generates reasonably fine-sounding and fairly diverse songs based on different initial notes we would call it a success.

### Milestone
Decide on the notes representation. There are many possible ways of notes representation e.g. treating note, its duration and offset as the word (possibly with some other measurements), we could also take only note and duration as the word and mark skipping to the new offset with special token and its duration, we could also add information of the duration or/and the offset with learnable offset/duration embeddings. Note representation might be determined by the chosen approach and architecture.

Preprocess data / create data preprocessing pipeline such that the new representation of notes will allow us to apply chosen approach on it.


