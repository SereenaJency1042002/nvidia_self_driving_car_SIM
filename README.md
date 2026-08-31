# Nvidia_self_driving_car_SIM

End-to-end deep learning model (NVIDIA PilotNet architecture) that learns to steer a car from front-facing camera images, trained via behavioral cloning in the Udacity self-driving car simulator.

## Dataset

Driving data sourced from [rslim087a/track](https://github.com/rslim087a/track).

## Setup

```bash
conda create -n nvidiacar python=3.7 -y
conda activate nvidiacar
pip install -r requirements.txt
```

## Run

1. Start the driving script:
```bash
python cardrive.py
```
2. Open the Udacity simulator and switch to **Autonomous Mode**.

The script listens on `localhost:4567` and streams steering/throttle predictions back to the simulator in real time.

## Files

- `nvidia_self_driving_car_model_NN.ipynb` — training notebook (Colab)
- `cardrive.py` — local driving script (loads trained model, connects to simulator)
- `model/` — saved model weights
- `requirements.txt` — dependencies
