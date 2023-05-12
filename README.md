
# Forest Fire Detection 🔥

Detecting forest fires using deep learning.

## Dataset

- [THE FLAME DATASET: AERIAL IMAGERY PILE BURN DETECTION USING DRONES (UAVS)](https://dx.doi.org/10.21227/qad6-r683)

## Models Used

- [DeepLabV3](https://pytorch.org/vision/main/models/deeplabv3.html)
- [LRASPP](https://pytorch.org/vision/main/models/lraspp.html)
- [Segformer](https://huggingface.co/docs/transformers/model_doc/segformer)

## Metrics

| Model | Params (M) | IoU | F1 |
| --- | --- | --- | --- |
| deeplabv3\_mobilenet\_v3\_large | 11.0 | 0.3544 | 0.5230 |
| deeplabv3\_resnet101 | 60.9 | 0.375 | 0.5450 |
| deeplabv3\_resnet50 | 42.0 | 0.3915 | 0.5623 |
| lraspp\_mobilenet\_v3 | 3.2 | 0.3713 | 0.5412 |
| segformer-b0 | 3.7 | 0.7446 | 0.8535 |
| segformer-b2 | 25.8 | 0.7671 | 0.8680 |
| ensemble | | 0.3724 | 0.5423 |

## Checkpoints

Checkpoints of the trained models are available in releases.

`segformer-b0` finetuned endpoint can also be found on [huggingface](https://huggingface.co/millionhz/segformer-b0-finetuned-flame).

## Installation and inference

- The notebooks will automatically download the self hosted dataset and checkpoints.
- The notebooks themselves are divided into subsections and are self-explanatory.
