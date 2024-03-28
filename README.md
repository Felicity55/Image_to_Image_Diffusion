### Install Requirements
Run the script:
```python
pip install -r requirements.txt
```

### Data Prepare
- [CelebA-HQ resized (256x256) Kaggle](https://www.kaggle.com/datasets/badasstechie/celebahq-resized-256x256)

### Training
Run the script:
```python
python run.py -p train -c config/twoImage.json
```

We test the U-Net backbone used in `SR3` and `Guided Diffusion`,  and `Guided Diffusion` one have a more robust performance in our current experiments.  More choices about **backbone**, **loss** and **metric** can be found in `which_networks`  part of configure file.

### Test
 Run the script:
```python
python run.py -p test -c config/twoImage.json
```


## Acknowledge
- [Palette: Image-to-Image Diffusion Models](https://arxiv.org/pdf/2111.05826.pdf)


