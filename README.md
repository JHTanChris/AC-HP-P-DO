# ACDOS-Software-Platform
Asphalt Concrete Design and Optimization System (ACDOS)
# Asphalt Concrete Design Optimization Software (ACDOS)

## Overview

The **Asphalt Concrete Design Optimization Software (ACDOS)** is an intelligent software platform for predicting and optimizing the high-temperature performance of asphalt concrete.
Developed using the **MATLAB R2024b App Designer**, ACDOS integrates data management, Gaussian Process Regression (GPR)–based machine learning prediction, and Bayesian Optimization algorithms into a unified graphical user interface (GUI).

The software consists of four core functional modules:

1. **Database Module (Database):** Enables efficient data storage, retrieval, and management.
2. **Model Construction Module (Model):** Builds and trains GPR-based prediction models for asphalt mixture performance.
3. **Performance Prediction Module (Prediction):** Provides intelligent forecasting of high-temperature performance parameters.
4. **Design Optimization Module (Optimization):** Implements Bayesian optimization to achieve optimal asphalt mixture designs.

ACDOS aims to bridge materials engineering and machine learning, providing researchers and engineers with a data-driven, automated, and highly visualized design tool for asphalt concrete performance evaluation and optimization.

---

## System Requirements

### Hardware Environment

ACDOS was developed and tested under the following configurations:

* **Development system:** 13th Gen Intel Core™ i5-13600KF, 32 GB RAM, NVIDIA GeForce RTX 4060 Ti
* **Testing system:** MacBook Pro (M4 chip, 16 GB RAM)

The software runs smoothly on both configurations. Computational efficiency may vary depending on user-defined parameters and hardware performance.

### Software Environment

* **Operating systems:** Windows 11 Professional and macOS Sequoia (15.3.1)
* **Programming language:** MATLAB
* **Development tool:** MATLAB R2024b (App Designer)
* **Required toolbox:** *Statistics and Machine Learning Toolbox* (v24.2)

> Note: ACDOS was built using **MATLAB R2024b**, and certain functions (e.g., `explainer = shapley()`, advanced plotting) may differ in earlier MATLAB releases. It is therefore recommended to run the software on **MATLAB R2024b or later** for full compatibility.

---

## Installation and Launch

1. **Prerequisite:**
   Ensure that **MATLAB R2024b** (or a later version) is installed on your system.

2. **Installation:**
   Download the provided ACDOS installation package (`ACDOS_V1.mlappinstall`).
   Double-click the file, or within MATLAB select:

   ```
   Home → Add-Ons → Install from File → ACDOS_V1.mlappinstall
   ```

   MATLAB will automatically install the app.

3. **Launch:**
   After installation, open MATLAB and navigate to the **App** tab.
   You will find **ACDOS V1** listed among installed apps.
   Click the icon to launch the GUI interface.

---

## Data Input

ACDOS V1.0 uses `.mat` files as the standard data format for consistent model training and prediction.

* **Loading Data:**
  In the *Data Load* panel, manually specify the local file path to your dataset.
  The data file should contain both input variables (**X**) and output responses (**Y**) saved in MATLAB `.mat` format.

* **Converting Data:**
  You may import any `.csv` or `.xlsx` dataset into MATLAB and convert it to `.mat` format using MATLAB’s **Import Data** function.
  This ensures full compatibility with the data management system of ACDOS V1.0.

---

## License and Citation

ACDOS has been registered under the **Computer Software Copyright of the People’s Republic of China**.
All rights reserved by the authors. The source code and compiled installer are made available for academic and research purposes only.
If you use ACDOS in your research, please cite the corresponding publication or this repository.
