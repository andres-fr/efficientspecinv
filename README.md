# Audio samples for our paper: "Efficient Neural and Numerical Methods for High-Quality Online Speech Spectrogram Inversion via Gradient Theorem"

* Website: https://anon782.github.io/audio_samples/
* Git repository: https://github.com/anon782/audio_samples

This webpage provides representative audio samples for clean speech data in WAV format.
Each row represents one random fragment from the Librispeech clean test split.
Each column represents a model used to generate the WAV directly from the STFT magnitude spectrogram:
* **Ground truth:** A perfect reconstruction via inverse STFT using ground truth magnitudes and phases
* **Proposed**: Our proposed method with efficient first and second stage
* **Prev. + Thomas**: The result of applying our proposed second stage to the [previously proposed CNN](https://ieeexplore.ieee.org/document/9944900)
* **Prev + direct**: The result of applying a direct solver to the [previously proposed CNN](https://ieeexplore.ieee.org/document/9944900)
* **VOCOS**: "Copy-synthesis" function using the VOCOS API and pretrained model, as prescribed in the [official repository](https://github.com/gemelo-ai/vocos)
* **RTISI (50 iter.)**: 50-iteration RTISI ([implementation](https://pypi.org/project/torch-specinv))
* **RTISI (5 iter.)**: 5-iteration RTISI ([implementation](https://pypi.org/project/torch-specinv))
* **Strided + LA**: The strided variation of our proposed method, with one frame of lookahead
* **Strided**: The strided variation of our proposed method, without lookahead

See our paper for more details.
