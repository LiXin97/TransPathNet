<div align="center">

<img width="22%" src="logo.webp" alt="TransPathNet logo">

# TransPathNet

### A Novel Two-Stage Framework for Indoor Radio Map Prediction

[Xin Li](https://lixin.ai/)¹, Ran Liu¹, Saihua Xu², Sirajudeen Gulam Razul², [Chau Yuen](https://blogs.ntu.edu.sg/chau-yuen/)¹<br>
¹ School of Electrical and Electronic Engineering, Nanyang Technological University, Singapore ·
² Temasek Laboratories @ NTU, Nanyang Technological University, Singapore

[![arXiv](https://img.shields.io/badge/arXiv-2501.16023-b31b1b?logo=arxiv)](https://arxiv.org/abs/2501.16023)
[![Project page](https://img.shields.io/badge/Project-page-059669)](https://lixin.ai/TransPathNet/)
[![Model](https://img.shields.io/badge/%F0%9F%A4%97%20Model-TransPathNet-ffcc4d)](https://huggingface.co/XINLI1997/TransPathNet)
[![Code license](https://img.shields.io/badge/code-MIT-blue)](LICENSE)

**A two-stage deep learning framework that predicts radio pathloss in indoor environments and generalizes to unseen
geometries, frequencies, and antenna patterns.**

</div>

## The idea in 30 seconds

- **The task.** Predict radio pathloss in challenging indoor environments, for the
  [Indoor Pathloss Radio Map Challenge](https://indoorradiomapchallenge.github.io).
- **The model.** TransPathNet integrates the [TransNeXt](https://github.com/DaiShiResearch/TransNeXt) model as the
  backbone and the [EMCAD](https://github.com/SLDGroup/EMCAD) module as the head, alongside custom modifications to
  excel in the competition tasks.
- **The three competition tasks.**
  1. **Task 1**: Generalization to new geometries.
  2. **Task 2**: Generalization to new geometries and frequencies.
  3. **Task 3**: Generalization to new geometries, frequencies, and antenna patterns.

## Main results

**TransPathNet** achieves state-of-the-art performance across all competition tasks. The weighted score is the overall
root mean squared error (RMSE, dB) on the challenge's full test set.

| Task 1 | Task 2 | Task 3 | Weighted score |
|:---:|:---:|:---:|:---:|
| 8.38 | 10.94 | 11.06 | 10.397 |

Check the competition [leaderboard](https://indoorradiomapchallenge.github.io/results.html) for detailed results.

## Quick start

To install the necessary dependencies, run the following command in your virtual environment:

```bash
pip install -r requirements.txt
```

- **Data:** download the dataset for training and evaluation from
  [IEEE DataPort](https://ieee-dataport.org/documents/indoor-radio-map-dataset).
- **Training:** the [training.ipynb](training.ipynb) notebook.
- **Evaluation:** the [evaluation.ipynb](evaluation.ipynb) notebook.

## Models and data

- **Pretrained model:** [🤗 TransPathNet](https://huggingface.co/XINLI1997/TransPathNet/tree/main).
- **Dataset:** [Indoor Radio Map Dataset](https://ieee-dataport.org/documents/indoor-radio-map-dataset) (IEEE DataPort).

## Repository layout

```
training.ipynb     training code
evaluation.ipynb   evaluation code
logo.webp          logo
LICENSE            MIT License
```

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

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

Third-party licenses:
- The backbone model, TransNeXt, is licensed under the Apache License 2.0. See `LICENSE-TransNeXt` for details.
- The head module, EMCAD, is licensed under the BSD 3-Clause License. See `LICENSE-EMCAD` for details.

## Contact

For any questions, please contact [xin019@e.ntu.edu.sg](mailto:xin019@e.ntu.edu.sg).
