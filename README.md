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
<<<<<<< HEAD
- Buzzer component:
  ![Buzzer](./hardware%20device%20module/buzzer.jpg)
- Device shape images:
  ![Device Shape](./hardware%20device%20module/shape.jpg)
=======
- Internal structure images (center control:nano 33 BLE sense & buzzer) ![Buzzer](./hardware%20device%20module/internal%20structure.jpg)
- Device shape images ![Buzzer](./hardware%20device%20module/shape.jpg)
>>>>>>> 

## Model Development
The project contains multiple model versions, from 1.0.5 to 1.0.10, showcasing the iterative process of model development. Key aspects include:
- Basic model versions
- Transfer learning versions
- Inference testing versions
- Stability testing tools

## Testing Environment
The testing environment is thoroughly documented with photos, such as:
- ![Testing Environment 1](./testing%20environment/0d9d5355084310baacfbe7fa18d0e9c.jpg)
- ![Testing Environment 2](./testing%20environment/c4585cea0cefe34963b1590a96a28a2.jpg)

## Data Collection
Photos of the data collection environment are provided to document the real-world application scenarios:
- ![Data Collection 1](./Photos%20of%20the%20data%20collection%20environment/ff2ff22afc49314b5a34ac375163de1.jpg)
- ![Data Collection 2](./Photos%20of%20the%20data%20collection%20environment/f939eb40fd6af8ab1cf4466c31eae90.jpg)
- ![Data Collection 2](./Photos%20of%20the%20data%20collection%20environment/df7fab5387dbd82f2cec2ae5920748b.jpg)


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
2. Model Selection: Choose the appropriate model version based on your needs (located in `export model` directory). Of all the trained models, ei-test2-arduino-1.0.8 was selected as the final deployment model based on the following considerations:

First, this version achieved a stable accuracy above 80% in the Model Testing section of Edge Impulse, while demonstrating relatively higher robustness in environments with small water flow and complex background noise (e.g., rain or human voice), compared to earlier versions such as 1.0.7. This indicates better generalization and a stronger ability to distinguish water flow sounds from ambient interference.

Second, when deployed on the Arduino Nano 33 BLE Sense board, the model maintained low-latency inference and fast response. With a conservative activation threshold set at 0.9 to reduce false positives, the model still effectively responded to strong water flow events. This suggests a good balance between usability and reliability in real-world applications.

Moreover, the model was trained using optimized MFE parameters, including a wider frequency range, increased filter count, and adjusted frame length. These configurations, supported by relevant literature and validated through experimentation, improved the feature extraction of water flow audio. By reducing the strength of data augmentation, the model was able to focus more on learning the true characteristics of water flow in realistic conditions.

Finally, deployment testing showed that the model maintained its recognition performance even after waterproof encapsulation, making it compatible with the actual use-case setup. Therefore, considering accuracy, robustness, inference performance, and deployability, ei-test2-arduino-1.0.8 is the most suitable model for this project.

For detailed training performance and feature space analysis, please refer to the weekly journal.
4. Testing and Validation: Use the methods in `testing environment` to validate the system.

## Notes
- Ensure the hardware devices are deployed in the correct order.
- Select the appropriate model version for deployment.
- Regularly check the system's operational status.
