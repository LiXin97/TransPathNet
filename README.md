# TransPathNet: A Novel Two-Stage Framework for Indoor Radio Map Prediction

<p align="center" width="100%">
    <img width="22%" src="./logo.webp">
</p>

--------
<p align="center">
	<a href="https://lixin.ai/TransPathNet/"><img src="https://img.shields.io/badge/TransPathNet-ProjectPage-green.svg"></a>
     <a href="http://...."><img src="https://img.shields.io/badge/TransPathNet-Paper-yellow.svg"></a>
</p>

This repository contains the implementation of **TransPathNet**, a novel two-stage deep learning framework designed for the **Indoor Pathloss Radio Map Challenge**. **TransPathNet** integrates the [TransNeXt](https://github.com/DaiShiResearch/TransNeXt) model as the backbone and the [EMCAD](https://github.com/SLDGroup/EMCAD) module as the head, alongside custom modifications to excel in the competition tasks. The network is built to predict radio pathloss in challenging indoor environments while generalizing to unseen geometries, frequencies, and antenna patterns.

## Competition Tasks

1. **Task 1**: Generalization to new geometries.
2. **Task 2**: Generalization to new geometries and frequencies.
3. **Task 3**: Generalization to new geometries, frequencies, and antenna patterns.

For competition details, visit the [official challenge page](https://indoorradiomapchallenge.github.io).

## Installation

To install the necessary dependencies, run the following command in your virtual environment:

```bash
pip install -r requirements.txt
```

## Dataset

The dataset used for training and evaluation can be downloaded from the following link: [Dataset URL](https://ieee-dataport.org/documents/indoor-radio-map-dataset)

### Training
Training code in the 'training.ipybn' notebook.

### Evaluation
Evaluate code in the 'evaluation.ipybn' notebook.

### Pretrained Model
Download the pretrained model from [this link](https://huggingface.co/XINLI1997/TransPathNet/tree/main).

## Results

**PathFormer** achieves state-of-the-art performance across all competition tasks:
- **Task 1**: 8.38
- **Task 2**: 10.94
- **Task 3**: 11.06
- **Weighted Score**: 10.397

Check the competition [leaderboard](https://indoorradiomapchallenge.github.io/results.html) for detailed results.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

### Third-Party Licenses
- The backbone model, TransNeXt, is licensed under the Apache License 2.0. See `LICENSE-TransNeXt` for details.
- The head module, EMCAD, is licensed under the BSD 3-Clause License. See `LICENSE-EMCAD` for details.

## Citation

If you find this work useful, please cite our paper:

```bibtex
@inproceedings{li2025transpathnet,
  title={TransPathNet: A Novel Two-Stage Framework for Indoor Radio Map Prediction},
  author={Li, Xin and Liu, Ran and Xu, Saihua and Razul, Sirajudeen Gulam and Yuen, Chau},
  booktitle={Proc. IEEE International Conference on Acoustics, Speech, and Signal Processing (ICASSP)},
  year={2025},
  month={April}
}
```

## Contact

For any questions, please contact [xin019@e.ntu.edu.sg](mailto:xin019@e.ntu.edu.sg).