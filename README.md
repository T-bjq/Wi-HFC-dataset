# Wi-HFC-dataset
## Overview  
This project presents the **Wi-Human-Fire Classification (Wi-HFC)** system, an innovative approach leveraging **Wireless Sensing Technology** for human-fire classification. Unlike traditional methods relying on cameras or sensors, Wi-HFC employs variations in **Received Signal Strength (RSS)** and **Channel State Information (CSI)** from wireless signals to detect fire and identify individuals in real-time. This approach offers significant advantages in terms of cost-effectiveness and adaptability, particularly in **Non-Line-of-Sight (NLOS)** environments such as high-rise buildings and complex indoor spaces.

## Key Features  
- **Dual-Mode Detection**: Integrates RSS- and CSI-based methods to achieve high classification accuracy across various scenarios.  
- **NLOS Capability**: Enables fire and human detection even through walls, overcoming the limitations of camera-based methods.  
- **High Efficiency**: Achieves an average classification accuracy of over **92%**, outperforming traditional deep learning models such as ResNet, MobileNet, and FCN.  
- **Cost-Effective Deployment**: Utilizes existing wireless infrastructure (Wi-Fi, Bluetooth, ZigBee) without requiring additional hardware.  
- **Flexible and Scalable**: Employs low-cost **ESP32 Wi-Fi SoCs** for data collection, making it suitable for large-scale deployment.

## How It Works  
- **Data Collection**: RSS and CSI data are collected using ESP32-based wireless fire sensors (WFS) deployed at different locations.  
- **Data Preprocessing**: RSS and CSI data are processed through filtering, subcarrier selection (for CSI), and augmentation techniques to ensure robustness.  
- **Feature Extraction**: A lightweight deep learning model with separable convolution blocks extracts key features while maintaining computational efficiency.  
- **Classification**: The processed data is classified into five categories, including scenarios with single or multiple individuals and fire presence.

## Experimental Setup and Results  
- **Scenarios**: Experiments were conducted in residential-like environments with varying distances (1m to 5m) between fire sources and wireless sensors.  
- **Performance**: The Wi-HFC system demonstrated superior accuracy, especially in complex environments. CSI-based detection achieved **high robustness** at longer distances, while RSS-based detection provided a **cost-effective solution** for simpler scenarios.  
- **Comparison**: Wi-HFC outperformed traditional deep learning models (ResNet, MobileNet, FCN) in classification accuracy and efficiency.  
- **Metrics**: The system was evaluated using standard metrics (accuracy, precision, recall) and proved effective with low computational and energy requirements.

## Advantages Over Traditional Methods  
- **Improved NLOS Detection**: Unlike cameras or infrared sensors, Wi-HFC can detect through obstacles, covering large areas without direct visibility.  
- **Cost-Effectiveness**: Utilizes readily available wireless networks, eliminating the need for expensive specialized hardware.  
- **Privacy Protection**: Ensures user privacy by avoiding video-based monitoring systems.  
- **Scalability**: Easily deployable in different environments without extensive infrastructure changes.

## System Architecture  
- **Wireless Signal Processing**: Explores changes in RSS and CSI caused by fire-related factors such as temperature rise and smoke.  
- **Lightweight Deep Learning Model**: Incorporates separable convolution blocks and residual connections for effective feature extraction with reduced computational complexity.  
- **Hardware Configuration**: ESP32 Wi-Fi SoCs are used for continuous real-time data collection and processing.

## Conclusion and Future Work  
The Wi-HFC system offers a **novel, cost-effective, and scalable solution** for human-fire classification, particularly in challenging NLOS environments. Future research will focus on improving algorithm adaptability, optimizing RSS-CSI fusion techniques, and extending the system to other applications, such as fall detection and activity recognition in smart environments.

## Contact Information  
For more details or questions, please contact the authors via the provided channels in the full paper.
