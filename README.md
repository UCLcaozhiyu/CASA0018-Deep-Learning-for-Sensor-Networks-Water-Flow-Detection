# CASA0018 Deep Learning for Sensor Networks - Water Flow Detection

## Project Overview
This project focuses on developing a deep learning-based sensor network for water flow detection. By utilizing machine learning models and sensor networks, the system aims to monitor and detect water flow status in real-time.

## Project Structure
```
├── hardware device module/     # Contains images and diagrams of the hardware device
├── testing environment/        # Photos of the testing environment
├── Photos of the data collection environment/  # Photos of the data collection environment
├── export model/              # Exported model files
│   ├── test2_inferencing1.0.7/
│   ├── Stability testing tool/
│   └── Multiple model versions
├── data set/                  # Data sets
├── best epochs/              # Best training epochs
└── weekly journal1.txt       # Project weekly journal
```

## Hardware Device
The project includes a comprehensive hardware device module, featuring:
- Internal structure images (e.g., `internal structure.jpg`)
- Buzzer component (`![Buzzer](hardware%20device%20module/buzzer.jpg)`)
- Device shape images (`shape.jpg`)

## Model Development
The project contains multiple model versions, from 1.0.5 to 1.0.10, showcasing the iterative process of model development. Key aspects include:
- Basic model versions
- Transfer learning versions
- Inference testing versions
- Stability testing tools

## Testing Environment
The testing environment is thoroughly documented with photos, such as `0fdcd1ccbe7c9c6e381b952ae33d69e.jpg`, to validate the system's real-world performance.

## Data Collection
Photos of the data collection environment are provided to document the real-world application scenarios.

## Technical Details and Progress
### Data Collection and Processing
- Utilized existing datasets and personally collected data for model training.
- Experimented with different parameter settings to optimize model performance.

### Model Training and Optimization
- Conducted multiple model training sessions, experimenting with different epoch settings and parameter adjustments, such as frame length, filter number, and FFT length.
- Employed data augmentation techniques, like time shift and noise injection, to enhance model robustness.

### Hardware Design and Testing
- Designed waterproofing solutions and conducted hardware testing, particularly with the newly acquired Arduino Nano 33 BLE.

### Challenges and Improvements
- Identified challenges with datasets and models, proposing improvements such as adding complex environmental sounds and adjusting frequency ranges.

### Future Plans
- Continue optimizing datasets and model parameters.
- Plan to include shower data in the dataset once waterproof design is complete.
- Plan to record data in the home kitchen to expand the dataset.

## Usage Instructions
1. Hardware Deployment: Refer to the device structure images in `hardware device module` for deployment.
2. Model Selection: Choose the appropriate model version based on your needs (located in `export model` directory).
3. Testing and Validation: Use the methods in `testing environment` to validate the system.

## Notes
- Ensure the hardware devices are deployed in the correct order.
- Select the appropriate model version for deployment.
- Regularly check the system's operational status.
