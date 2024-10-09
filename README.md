
# United Airlines Call Center Optimization

*Dataset Link* : https://drive.google.com/drive/folders/16iBX-rtiBChaB-x3P5_YeZE-v3bRfTFi?usp=drive_link 

## Project Overview

This project focuses on optimizing key call center metrics, specifically Average Handle Time (AHT) and Average Speed to Answer (AST), to help United Airlines improve its customer service. The goal is to analyze the call center data, identify inefficiencies, and provide actionable strategies to enhance operational efficiency and customer satisfaction.

## Problem Statement

United Airlines seeks to reduce AHT and AST to improve call center operations, which are essential for providing world-class customer service. This project involves:
- Analyzing existing call center data.
- Identifying inefficiencies and the drivers of long AHT and AST.
- Suggesting improvements to streamline processes, reduce escalations, and enhance the overall customer experience.

### Key Metrics
- **AHT** (Average Handle Time): Time from when the agent picks up the call to when they hang up.
  - Formula: `AHT = Total Handle Time / Total Number of Calls`
- **AST** (Average Speed to Answer): Time spent by the customer in the queue before the agent answers the call.
  - Formula: `AST = Total Waiting Time / Total Number of Calls`

## Datasets Used
- **calls.csv**: Contains information about calls, including call start and end times.
- **customers.csv**: Contains customer information, such as customer ID and loyalty status.
- **sentiment_statistics.csv**: Provides sentiment scores for each call.
- **reason.csv**: Contains the primary reason for each call.

## Features
- **Average Handle Time (AHT) and Average Speed to Answer (AST)**: Calculated to assess the overall efficiency of the call center.
- **Sentiment Analysis**: Analyzes agent and customer sentiment during calls.
- **Call Clustering**: Uses TF-IDF and K-Means clustering to group call transcripts and identify recurring issues.
- **IVR System Optimization**: Proposes improvements to the IVR system to reduce agent escalations for common issues.

## How to Run the Project

### Prerequisites
1. **Python 3.x** installed on your system.
2. Libraries:
   - `pandas`
   - `numpy`
   - `matplotlib`
   - `seaborn`
   - `nltk`
   - `sklearn`
3. The project can be run in **Jupyter Notebook** or **Google Colab**.

### Running the Code

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/united-airlines-call-center.git
   cd united-airlines-call-center
   ```

2. **Install required libraries**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the Jupyter notebook**:
   - If you're using Jupyter Notebook, open the `.ipynb` file:
     ```bash
     jupyter notebook United_Airlines.ipynb
     ```
   - If you're using Google Colab:
     1. Upload the `.ipynb` file to your Google Drive.
     2. Open it in Google Colab.

4. **Data Files**:
   Ensure that all CSV files (`calls.csv`, `customers.csv`, `reason.csv`, `sentiment_statistics.csv`) are placed in the same directory as the notebook.

### Key Code Sections

- **Data Loading and Merging**: Loads and merges the datasets.
- **Metric Calculation**: Calculates AHT and AST, including their breakdown by call reason.
- **Data Visualization**: Provides various visualizations to explore AHT, AST, and sentiment.
- **Call Clustering**: Identifies common themes in call transcripts using K-Means clustering.
- **IVR Optimization**: Proposes improvements to reduce unnecessary agent escalations.

### Optional Task
To predict the primary call reason from the `test.csv` file, follow these steps:
1. Place `test.csv` in the project directory.
2. Run the section for generating predictions.
3. The output will be saved as `test_<name>.csv`.

## Deliverables

- **Code Files**: Submitted along with instructions to run them.
- **Presentation**: A concise data-driven presentation in `.ppt` format summarizing findings and recommendations.
- **(Optional)**: Predictions in `test_<name>.csv` format.

## Authors

- Belo Abhigyan
- Rajat Sharma

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

This `README.md` provides a clear structure and instructions for your project. Feel free to modify it further based on your specific needs!
