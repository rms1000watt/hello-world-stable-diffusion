# Hello World Stable Diffusion

## Introduction

Follow the guide here: https://replicate.com/blog/run-stable-diffusion-on-m1-mac

## Contents

- [Setup](#setup)

## Setup

From the guide here: https://replicate.com/blog/run-stable-diffusion-on-m1-mac

```bash
git clone -b apple-silicon-mps-support https://github.com/bfirsh/stable-diffusion.git
cd stable-diffusion
mkdir -p models/ldm/stable-diffusion-v1/

python3 -m pip install -r requirements.txt

python scripts/txt2img.py \
  --prompt "a red juicy apple floating in outer space, like a planet" \
  --n_samples 1 --n_iter 1 --plms

python scripts/txt2img.py \
  --prompt "Napolean Dynomite using a Windows 95 Compaq computer with a plate of nachos at his desk" \
  --n_samples 1 --n_iter 1 --plms
```