# Hello World Stable Diffusion

## Introduction

From the guide here: https://replicate.com/blog/run-stable-diffusion-on-m1-mac & clone of https://github.com/bfirsh/stable-diffusion

## Contents

- [Run](#Run)

## Run

- Read the guide above to get the model and place it in the right spot.
- Then install brew deps.
- Then run the script.

```bash
brew install protobuf cmake rust

python3 -m pip install -r requirements.txt

python3 scripts/txt2img.py \
  --prompt "a red juicy apple floating in outer space, like a planet" \
  --n_samples 1 --n_iter 1 --plms

python3 scripts/txt2img.py \
  --prompt "Programmer using a Windows 95 Compaq computer with a plate of nachos at his desk" \
  --n_samples 1 --n_iter 1 --plms
```
