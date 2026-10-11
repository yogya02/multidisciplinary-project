# Wildfire Detection from Satellite Images

A deep learning project that classifies satellite images as wildfire / no-wildfire, inspired by a research paper on early wildfire detection from GOES-16 satellite data. Built as our Basic Multidisciplinary Project (BAXXX191).

## Base paper
Nguyen, T. T., Phan, T. C., Nguyen, Q. V. H., & Jo, J. (2019). *A deep learning approach for early wildfire detection from hyperspectral satellite images.* 2019 7th International Conference on Robot Intelligence Technology and Applications (RiTA), IEEE, pp. 38-45.

The paper proposes a 3D-CNN that classifies each pixel of GOES-16 imagery as fire or no-fire, plus a streaming pipeline and a monitoring dashboard. Our project is a scaled-down version: a CNN-based image classifier trained on a public satellite dataset, with a simple web app for predictions.

## Project goals
1. Prepare a satellite-image dataset for wildfire classification (cleaning, resizing, normalization, augmentation, train/validation/test split).
2. Train a CNN (or a transfer-learning model such as MobileNetV2) to classify images as wildfire or no-wildfire.
3. Evaluate it with precision, recall and F1-score, and compare it against a simple baseline.
4. Build a Streamlit app where a user uploads an image and gets a prediction.

## Team
| Member | Role |
|---|---|
| Yogya | Team lead and environment |
| Pavan | Data acquisition and literature review |
| Rohan | Exploratory data analysis |
| Rounak | Preprocessing |
| Rithanya | Augmentation, splits and documentation |

## Dataset
- **Name:** Wildfire Prediction Dataset (Satellite Images)
- **Source:** [Kaggle link]
- **Licence:** [licence shown on the Kaggle page]
- **Size:** 42,850 images (350x350 pixels), two classes: wildfire (22,710) and no-wildfire (20,140)
- **Note:** The labels mark areas that previously experienced wildfires, so this is closer to "wildfire-affected area" classification than live flame detection. The base paper detects active fires at pixel level.

The dataset and trained models are stored in Google Drive, not in this repository, because of their size.

**Shared Drive folder:** [Drive link]

## Repository structure
```
wildfire-detection
├── notebooks   # Colab notebooks, one per pipeline stage
├── report      # Reports and presentations
├── results     # Charts and graphs
└── README.md
```

## Environment
- Platform: Google Colab (GPU enabled)
- Python: [version]
- TensorFlow / Keras: [version]
- OpenCV: [version]

## Timeline
| Review | Date | Scope |
|---|---|---|
| Review-I | 23 Oct 2026 | Setup, dataset, exploration, preprocessing, augmentation and split |
| Review-II | 22 Jan 2027 | Trained model, evaluation and a basic app |
| Review-III | 12-16 Apr 2027 | Complete project, demo and report |

## Progress
- [ ] Environment and repository setup
- [ ] Dataset downloaded and documented
- [ ] Data exploration
- [ ] Preprocessing
- [ ] Augmentation and train/validation/test split
- [ ] Model training
- [ ] Evaluation against baseline
- [ ] Streamlit app
- [ ] Final report
