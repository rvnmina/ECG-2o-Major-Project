ECG2o is an innovative project developed by a team of four under the mentorship of Professor. It is designed to revolutionize cardiac diagnostics by integrating cutting-edge digital signal processing techniques, robust machine learning algorithms, and real-time cloud connectivity. This system processes raw ECG data acquired from an Arduino-ESP8266 module, enabling precise detection and classification of arrhythmic events.


**Project Overview**


**Raw Data Acquisition**: The heart of ECG2o lies in capturing high-fidelity raw ECG signals using an Arduino-ESP8266 platform. This hardware setup enables wireless transmission of the raw data, providing a reliable foundation for subsequent processing steps.

**Advanced Signal Processing**: The acquired data undergoes sophisticated noise suppression and signal enhancement techniques—including digital filtering and wavelet transforms—to isolate critical features such as the QRS complex and R-peaks.

**Machine Learning Integration**: Extracted features are analyzed with advanced machine learning classifiers to detect and categorize arrhythmias with high accuracy.

**Real-Time Visualization**: Processed data is transmitted to a Firebase cloud backend and displayed on an interactive React.js dashboard, ensuring clinicians have immediate access to actionable diagnostic information.


**Technical Architecture**


**1. Data Acquisition:**

**·** Utilizes an Arduino-ESP8266 module to capture raw ECG signals.

**·** Transmits the data wirelessly to a cloud storage solution (Firebase) for real-time processing.


**2. Preprocessing:**

**·** Implements state-of-the-art filtering techniques and wavelet-based noise reduction to enhance signal quality.


**3. Feature Extraction & Classification:**

**·** Extracts key ECG features (e.g., QRS complex, R-peaks).

**·** Applies machine learning models to accurately classify various arrhythmic conditions.


**4. Visualization:**

**·** Uses a React.js-based dashboard to provide real-time visualization of the processed ECG waveform and diagnostic metrics.


**How to Use ECG2o**

This project uses an Arduino UNO and AD8232 sensor to build an affordable, real-time ECG monitor with simple, off-the-shelf components.

1. **Arduino UNO** is the main microcontroller that reads analog signals from the AD8232 sensor, converts them to digital data, and sends them to the display for continuous, real-time heart monitoring.

![image](https://github.com/user-attachments/assets/ef905db9-44dd-4c2c-b419-06df43976a82)




2. The **AD8232** is a bio-potential sensor that extracts, amplifies, and filters weak cardiac signals to clearly capture the PQRST waveform for ECG monitoring.

![image](https://github.com/user-attachments/assets/34bc07dc-c69e-4be7-8260-e2ee4a3ff2c8)




3. The** TFT SPI display** renders the real-time ECG data by graphically showing the PQRST waveform via the Arduino's SPI interface, ensuring even small signal fluctuations are clearly captured.

![image](https://github.com/user-attachments/assets/8dccc8e2-1ba1-4ccd-a657-61ef1df0c88a)



4. **Three electrodes** placed on the left chest, right chest, and right abdomen capture the heart's bio-potential and transmit the signals to the AD8232 sensor for processing.

![image](https://github.com/user-attachments/assets/9754e8cc-5c4a-4b97-a9c9-3fd514554c53)



5. **Resistors** match the impedance of SPI lines, reducing reflections and degradation while filtering high-frequency noise and limiting crosstalk—crucial for clear ECG signal acquisition.

![image](https://github.com/user-attachments/assets/9b2207ed-ea10-403d-b198-532a0b1b6cf8)



6. The **circuit integrates** the AD8232 sensor, noise-minimizing resistors, an Arduino UNO, and a TFT SPI display to capture, filter, and amplify heart signals, then render the PQRST ECG waveform in real time for continuous monitoring.

![image](https://github.com/user-attachments/assets/12cc9ae6-17af-49b7-b3db-8143edbe3d8a)


**METHODOLOGY**

**A. Hardware Setup:**  

The system connects the AD8232 sensor to the Arduino UNO, with three electrodes placed on the left chest, right chest, and right abdomen to capture the heart’s signals, which are then processed and displayed in real time.

![image](https://github.com/user-attachments/assets/57d013d1-83a3-432e-939c-ce79b105be6a)


**B. Signal Acquisition:**

Once the electrodes are attached, the AD8232 sensor captures the biopotential signals and filters out any muscle or environmental noise. The sensor’s output is an amplified ECG signal, which is then sent to the Arduino for further processing.

![image](https://github.com/user-attachments/assets/c1615d1a-f074-45a5-b9b1-20078bd14b72)


**C. Data Processing:**

The Arduino converts the analog signals from the sensor into digital data that can be displayed on the TFT SPI display. The Arduino IDE's serial monitor also captures these signals, allowing for dual visualization of the ECG waveform..

![image](https://github.com/user-attachments/assets/2857ca4a-8977-48a3-9a02-326779ed0e5d)


**D. Ensuring Signal Clarity:**

The resistors in the circuit play a crucial role in reducing electrical noise, ensuring that the ECG signals captured from the heart are
clear and undistorted. By controlling the flow of current, the resistors prevent interference and noise from affecting the signals,
allowing the PQRST waveform to appear clearly on the display

![image](https://github.com/user-attachments/assets/c370988a-7886-4405-b04f-fb57994a30c5)




**RESULTS AND OBSERVATIONS -**

The system successfully displayed real-time ECG signals on both the TFT SPI screen and the Arduino IDE serial monitor, with the
PQRST waveform clearly visible and the signal clarity maintained throughout the monitoring process. Thanks to the resistors used
for noise reduction, the system proved capable of continuous and stable monitoring. This makes it suitable for educational and
personal healthcare applications. The real-time ECG signals demonstrated clear PQRST waveforms, indicating that the system could
accurately capture and display heart signals.


![image](https://github.com/user-attachments/assets/7b3569e6-fc05-4711-ad64-f0323b626123)



****How to Run****

Clone this repository. Open the Arduino IDE. Install necessary libraries. Configure the code with your credentials. Upload the code to your ESP8266 board. Monitor the serial console for connection status.

