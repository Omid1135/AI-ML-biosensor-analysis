# AI-ML-biosensor-analysis
Comprehensive dataset (5000 spectra) of simulated grating biosensor reflections in Excel format. Generated via Lumerical FDTD, it includes 11 parameters (thickness, RI, peak wavelength, FWHM, reflectance, etc.). It is ideal for data visualization, sensor response exploration, and AI/ML benchmarking. 
The full dataset in Excel format is coming soon!  Follow this repository to be notified when it's released.  In the meantime, feel free to browse the README for more information about the project.

--------- Description of the Research -------

This study presents a Python-driven approach for analyzing optical biosensor data by combining Finite-Difference Time-Domain (FDTD) simulations with Artificial Intelligence (AI) and Machine Learning (ML).  Addressing the challenge of limited experimental data, I generated a comprehensive dataset using Lumerical FDTD simulations of an optical biosensor.

Methodology Summary:

--Sensor Design & FDTD Simulation: A  resonant optical biosensor, based on an experimental design, was modeled and simulated using Lumerical FDTD. Importance: Accurate FDTD simulations are essential for modeling the complex electromagnetic interactions within the sensor and generating realistic data.

-- Parametric Study:  A parametric study was conducted by varying the analyte. This resulted in 5000 simulated reflection spectra. Importance: Systematically varying analytes created a diverse dataset representative of different analyte conditions, which is crucial for training robust AI/ML models.

-- Data Processing & Feature Extraction (Python):  A custom Python script was developed to process the raw simulation data. This script extracted key spectral features from each spectrum. These features were compiled into an Excel file.

-- Advanced data Visualization & Analysis (Python): Python libraries like Pandas, NumPy, and Matplotlib were used for advanced data visualization and analysis. This revealed insights into sensor behavior, including sensitivity enhancement and complex variations in the sensitivity coefficient.  Importance: Advanced visualizing the data allows for identifying trends, anomalies, and complex relationships that may not be apparent from raw numerical data.  This step was crucial for understanding the sensor's response to different analyte conditions.

-- Machine Learning (Python): A Multi-Layer Perceptron (MLP) model, implemented using Scikit-learn, was trained to predict sensor results.  The MLP architecture consisted of an input layer, five hidden layers (100 neurons each), and an output layer.  ReLU activation and the Adam optimizer were used.  The model was trained for 1000 epochs with L2 regularization.  Importance: Machine learning allows for modeling complex, non-linear relationships between sensor input parameters and output spectral features, going beyond traditional single-parameter analysis.

-- Model Evaluation: The trained MLP model was evaluated on a test dataset.  Performance metrics, including Mean Squared Error (MSE), R-squared, and Pearson correlation coefficient, were calculated to assess the model's accuracy in predicting sensor parameters. Importance: Rigorous model evaluation is essential to ensure the reliability and generalizability of the trained AI/ML model.
