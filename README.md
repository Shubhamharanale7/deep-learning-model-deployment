# Deep Learning Model Deployment with YOLOv3 & FastAPI

A hands-on project where I deployed a computer vision model capable of identifying and localizing common objects in images. Built using the YOLOv3 object detection model and served via FastAPI through Jupyter notebooks.

**Built by:** Shubham Haranale

---

## What This Project Does

This project demonstrates the full pipeline of taking a pre-trained deep learning model (YOLOv3) and deploying it as a working API service:

- **Server** (`server.ipynb`) — Loads the YOLOv3 model and exposes it as a FastAPI endpoint that accepts images and returns predictions with bounding boxes
- **Client** (`client.ipynb`) — Sends images to the server and displays the results with detected objects highlighted

---

## What I Learned

- How to serve a deep learning model as a REST API using **FastAPI**
- The difference between a model **training** environment and a model **serving** environment
- How to structure a client-server architecture for ML inference
- Managing Python dependencies and virtual environments for ML projects
- Practical MLOps concepts from Andrew Ng's MLOps Specialization (DeepLearning.AI)

---

## Project Structure

```
.
├── images/                  # Sample input images (from ImageNet)
├── images_uploaded/         # Images sent to the server
├── images_predicted/        # Output images after inference
├── images_with_boxes/       # Images with bounding boxes drawn
├── assets/                  # Supporting assets
├── server.ipynb             # FastAPI server with YOLOv3 model
├── client.ipynb             # Client to send requests to the server
└── requirements.txt         # Python dependencies
```

---

## Setup & Running Locally

### 1. Create a virtual environment

```bash
conda create --name dl-deploy python=3.8
conda activate dl-deploy
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Launch Jupyter Lab

```bash
jupyter lab
```

### 4. Run the notebooks

- Open and run **`server.ipynb`** first to start the FastAPI server
- Then open and run **`client.ipynb`** to send images and see predictions

---

## Tech Stack

- **Model:** YOLOv3 (object detection)
- **API Framework:** FastAPI
- **Environment:** Jupyter Lab, Conda, Python 3.8
- **Concepts:** MLOps, model serving, REST API, client-server architecture

---

## Acknowledgement

Project inspired by the [Machine Learning Engineering for Production (MLOps) Specialization](https://www.deeplearning.ai/courses/machine-learning-engineering-for-production-mlops/) by Andrew Ng, Laurence Moroney, and Robert Crowe on DeepLearning.AI.


To stop jupyter lab once you are done with the lab just press `Ctrl + C` twice.

### And... that's it! Have fun deploying a Deep Learning model! :)

Based on [Machine Learning Engineering for Production (MLOps) Specialization](https://www.deeplearning.ai/courses/machine-learning-engineering-for-production-mlops/) by Andrew Ng, Laurence Moroney, and Robert Crowe (2023).
