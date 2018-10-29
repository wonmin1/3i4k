# 3i4K
Intonation-aided identification of intention for Korean

## Requirements
fastText, Keras (TensorFlow), Numpy

## Word Vector
[Pretrained 100dim fastText vector](https://drive.google.com/open?id=1jHbjOcnaLourFzNuP47yGQVhBTq6Wgor)
* Download this and unzip THE .BIN FILE in the same folder with 'onlychar_fast_execute.py'.
* This can be replaced with whatever model the user employs, but it requires an additional training.

## System Description
* Easy start: Python3 execute file
<pre><code> python3 onlychar_fast_execute.py </code></pre>

### Intention Identification
 - First, this system detects the fragments.
 - Next, if the input sentence clearly shows its intention among statement, question, command, rhetorical question and rhetorical command (idiomatic expression), this directly decides the intention.
 - If the intonation information is indispensable, this requires an auxiliary feature and makes an intonation-aided decision.
 
### Text Classification
 - This system classifies a corpus (input: filename without '.txt') into 7 categories: fragments, intonation-dependent utterances, and previously mentioned 5 clear-cut cases.

## Annotation Guideline (in Korean)
https://drive.google.com/open?id=1AvxzEHr7wccMw7LYh0J3Xbx5GLFfcvMW

## YouTube demo (non-audio-input version)
https://youtu.be/OlvLlH8JgmM
