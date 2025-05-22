# Istanbul Technical University Graduation Thesis: Metro Istanbul Usage Prediction Using with Digital Twin Approach 

This repository contains my graduation thesis, a research paper focused on **predicting Metro Istanbul usage with smart card data**. This work leverages machine learning models developed and executed on Kaggle Servers.

## Overview

This thesis explores the application of machine learning to forecast passenger numbers for Istanbul's metro system. The primary objective is to enhance urban mobility by providing predictive insights for operational planning and optimizing the metro network's response to changing demand.

## Research Focus

The research addresses the challenge of predicting urban transportation demand in a rapidly growing metropolis. It investigates the effectiveness of Long Short-Term Memory (LSTM) networks in time-series forecasting of passenger flow, utilizing smart card transaction data.

## Methodology

The research employed a data-driven approach using:

* **Data:**
    * https://data.ibb.gov.tr/datarequest
    * Metro Istanbul rail system daily/monthly/yearly line-based trip counts: <https://data.ibb.gov.tr/rayli-sistemler-gunluk-aylik-yillik-hat-bazli-sefer-sayilari/> (Accessed: 10.05.2025)
    * Istanbul dams daily total rainfall amount (auxiliary data): <https://data.ibb.gov.tr/dataset/istanbul-barajlarina-dusen-gunluk-toplam-yagis-miktari/> (Accessed: 19.05.2025)
    * Smart card transaction data (primary source).
* **Tools:** Python, Pandas, TensorFlow/Keras, and other relevant libraries.
* **Environment:** All models and analyses were performed within a Kaggle notebook environment.

## System/Process Flow

The `Structure_Flow.jpg` image illustrates the overall process of this research, from data acquisition and analysis to model design, performance evaluation, and prediction.

<div align="center">
  ![Flow Diagram](flow.png)
</div>

## Key Findings

* The LSTM model demonstrated strong performance in predicting hourly passenger numbers.
* Achieved a **Root Mean Squared Error (RMSE) of approximately 263 passengers**, indicating the average magnitude of prediction errors.
* The model explained **approximately 82% of the variance (R²)** in passenger numbers, showcasing its efficiency in utilizing data for prediction.
* Identified key factors influencing metro usage, such as seasonality (weekdays vs. weekends) and peak usage during morning and evening rush hours.

## Getting Started

To explore the project:

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/yasinnerten/graduation-thesis.git
    cd graduation-thesis
    ```
2.  **Access the model:** The core model and analysis are in the [Jupyter Notebook] (Metro_Istanbul_Usage_Prediciton.ipynb). You can open it directly on Kaggle for an interactive experience.
3.  **Review the thesis document:** The full research paper will be publish by Coperman after the conference.

## How to Run the Model (for Contributors)

If you wish to run the model locally and contribute, follow these steps:

1.  **Ensure Python is installed:** Make sure you have Python 3.8+ installed on your system.
2.  **Create a virtual environment:** It's highly recommended to use a virtual environment to manage dependencies.
    ```bash
    python3 -m venv venv
    ```
3.  **Activate the virtual environment:**
    * On Linux/macOS:
        ```bash
        source venv/bin/activate
        ```
    * On Windows:
        ```bash
        .\venv\Scripts\activate
        ```
4.  **Install required packages:** All necessary Python packages are listed in the `Metro_Istanbul_Usage_Prediciton.ipynb` notebook (typically at the beginning, in cells containing `pip install` or `conda install` commands). Identify these and install them within your activated virtual environment. For example:
    ```bash
    pip install pandas numpy tensorflow scikit-learn matplotlib seaborn jupyter
    ```
    (Adjust the list of packages based on the actual notebook content).
5.  **Launch Jupyter Notebook:**
    ```bash
    jupyter notebook Metro_Istanbul_Usage_Prediciton.ipynb
    ```
6.  **Run the cells:** Once the Jupyter Notebook opens in your browser, you can execute the cells sequentially to reproduce the data processing, model training, and evaluation.

## Repository Structure

* `Metro_Istanbul_Usage_Prediciton.ipynb`: Jupyter Notebook containing the data processing, model training, and evaluation.
* `Structure_Flow.png`: Visual representation of the research workflow.
<!-- * `AhmetYasin_DevelopingaDigitalTwinSystemforPredictingUsageofIstanbulMetro.pdf`: The complete graduation thesis document. -->
* `[Dataset/]`: Raw or processed datasets.

## Contact

For any questions or collaborations, please contact:

* **Ahmet Yasin Erten**
* **Email:** ertena19@itu.edu.tr
* **GitHub:** [@yasinnerten](https://github.com/yasinnerten)
* **Linkedin:** https://www.linkedin.com/in/yasinnerten/
## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
