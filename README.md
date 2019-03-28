This repository hosts code and document for the [RecSys Challenge 2018](http://www.recsyschallenge.com/2018/),
the task is about music playlist continuation using the [Million Playlist Dataset (MPD)](https://recsys-challenge.spotify.com/).
This work adopts a matrix factorisation approach to learn latent representations of songs and playlists,
it minimises the Top Push Loss (see `code/Train.ipynb` for details) for each playlist in the MPD.

To make use of this work, uncompress the MPD data and put the JSON files in `data/mpd`,
put the challenge set JSON file in `data` and run the Jupyter notebooks in `code`
in the following order:

1. `Preprocess.ipynb`, run this notebook to convert the data in JSON files into Python data structures,

2. `Train.ipynb`, run this notebook to learn the latent representations of songs and playlists,

3. `Recommend.ipynb`, run this notebook to make recommendations for playlists in the challenge set.



Required libraries:

- [Python](https://www.python.org/), version 3.6
- [Numpy](http://www.numpy.org/), version 1.14.3
- [Scipy](https://scipy.org/scipylib/index.html), version 1.1.0
- [Tensorflow](https://www.tensorflow.org/), version 1.8.0
- [PyTorch](https://pytorch.org/), version 0.4.0
- [Jupyter](http://jupyter.org/index.html), version 1.0
- [tqdm](https://pypi.org/project/tqdm/), version 4.23.4



Copyright 2018 Dawei Chen. All Rights Reserved.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
