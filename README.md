# Beyond the Beep: Enhancing Customer Experience Through Smarter Call Center Operations

*Dataset Link*: [Google Drive](https://drive.google.com/drive/folders/16iBX-rtiBChaB-x3P5_YeZE-v3bRfTFi?usp=drive_link)

*PPT Link*: [Click Here](https://docs.google.com/presentation/d/1DgbHzziqg_F074ixru4xupcuE2d0Z__Z/edit?usp=sharing&ouid=114321354679631077001&rtpof=true&sd=true)

*PDF Link*: [Click Here](https://drive.google.com/file/d/1sA6AbNzj3BUxHa_q6lePm8BixXkbA0KT/view?usp=sharing)

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

## Approach

To achieve the project objectives, I employed the following approach:

1. **Data Collection and Preprocessing**: 
   - Gathered datasets relevant to call center operations and merged them into a unified DataFrame for comprehensive analysis. 
   - Cleaned the data to handle missing values and ensure its accuracy.

2. **Metric Calculation**: 
   - Calculated AHT and AST, breaking them down by call reasons to understand the factors impacting efficiency.

3. **Exploratory Data Analysis (EDA)**: 
   - Conducted correlation analysis and visualizations to identify relationships between variables such as sentiment, waiting times, and handling times.
   - Analyzed trends in call reasons and their associated AHT to uncover inefficiencies.

4. **Natural Language Processing (NLP)**: 
   - Utilized NLTK for preprocessing call transcripts, including tokenization and removing stopwords.
   - Employed TF-IDF vectorization to convert textual data into numerical features for further analysis.

5. **Clustering Analysis**: 
   - Applied K-Means clustering to identify recurring themes in call transcripts, which highlighted areas where IVR improvements could be made.

6. **Predictive Modeling**: 
   - Developed a logistic regression model to predict primary call reasons based on historical call data, enabling proactive resource allocation and improved customer service.

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
