# TerrainGuard: Smart Landslide Detection and Alert System

## Table of Contents
- [About the Project](#about-the-project)
- [System Architecture](#system-architecture)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Methodology](#methodology)
- [Dataset](#dataset)
- [Evaluation](#evaluation)
- [Future Work](#future-work)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## About the Project
**TerrainGuard** is an IoT-powered, AI-driven landslide detection and alert system. Utilizing a combination of environmental sensors (rain gauges, inclinometers, seismic sensors) and a deep learning LSTM model, TerrainGuard aims to predict landslide risks. This system enhances landslide monitoring and early warning capabilities to protect lives, infrastructure, and communities in landslide-prone areas.

## System Architecture
The architecture of TerrainGuard consists of three primary components:

1. **Sensor Network**: An IoT-based network of sensors to capture environmental data, including rainfall, ground tilt, and seismic activity.
2. **Data Processing Hub**: A central processing unit that aggregates data and uses a deep learning model to assess landslide risks, triggering alerts if necessary.
3. **Communication Module**: Utilizes LoRaWAN for reliable long-range data transmission, especially useful for remote regions susceptible to landslides.

## Features
- **Real-Time Monitoring**: Continuous tracking of rainfall, ground tilt, and seismic activity.
- **Landslide Prediction**: Predictive analytics using an LSTM model to detect landslide indicators in time-series data.
- **Early Warning Alerts**: Sends notifications to relevant authorities and at-risk communities.
- **Explainable AI (XAI)**: Provides interpretable insights for actionable model predictions.

## Installation

To set up TerrainGuard locally, follow these steps:

1. **Clone the Repository**
   ```bash
   git clone https://github.com/username/TerrainGuard.git
   cd TerrainGuard
   ```

2. **Install Dependencies**  
   Make sure Python and pip are installed, then run:
   ```bash
   pip install -r requirements.txt
   ```


### Real-Time Monitoring and Alerts
Deploy the system and configure alerts via SMS or app notifications using services like Twilio or Firebase.

## Methodology
TerrainGuard leverages a Long Short-Term Memory (LSTM) network to model temporal dependencies within environmental data, enabling accurate predictions of landslide risks. The model analyzes sequential patterns in rainfall, ground tilt, and seismic activity to assess risk levels.

For further details, refer to the **Methodology Document**, which provides an in-depth explanation of the deep learning architecture and sensor fusion techniques.

## Dataset
The custom dataset includes the following key features:

- **Rainfall**: Recorded in millimeters (mm) to indicate precipitation levels.
- **Tilt Angle**: Measures ground inclination.
- **Seismic Activity**: Captures ground vibrations.
  
Each dataset entry is labeled with a binary target: `1` for landslide occurrence, `0` for no landslide. This dataset can be extended with additional environmental factors to improve model accuracy.

## Evaluation

**Model Metrics**:
- **Accuracy**: 98%
- **Precision**: 97%
- **Recall**: 96%
- **F1-Score**: 98%

**Evaluation Visualizations**:
- **Confusion Matrix**
- **ROC Curve**
- **Precision-Recall Curve**

These metrics and visualizations demonstrate the model's efficacy in predicting landslides. For a detailed analysis, refer to the **Evaluation Results**.

## Future Work
Upcoming improvements include:

- **Hybrid Deep Learning Models**: Exploring CNN-LSTM combinations for enhanced spatial-temporal analysis.
- **Satellite and Drone Data Integration**: Adding real-time data from satellite imagery and drone surveillance.
- **Explainable AI Tools**: Utilizing SHAP or LIME for improved feature interpretability.
- **User Studies**: Validating system performance in real-world deployments.

## Contributing
We welcome contributions to TerrainGuard! Please follow our contribution guidelines and submit your pull requests.

## License
Distributed under the MIT License. See `LICENSE` for more information.

## Contact
Lead Researchers:
- **Balaji Ganesh Rajagopal** - [balajiganesh.r@ist.srmtrichy.edu.in](mailto:balajiganesh.r@ist.srmtrichy.edu.in)
- **Jagadeesh Kannan Raju** - [dr_rjk@hotmail.com](mailto:dr_rjk@hotmail.com)


