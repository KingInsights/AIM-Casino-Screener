# AIM Casino Screener Significant Decline

## Table of Contents
- [Introduction](#introduction)
- [Setup](#setup)
  - [Running the Notebook Locally with Jupyter Lab](#running-the-notebook-locally-with-jupyter-lab)
  - [Running the Notebook Online with Google Colab](#running-the-notebook-online-with-google-colab)
- [Running the Project](#running-the-project)
- [Acknowledgments](#acknowledgments)
- [License](#license)

## Introduction
This project aims to identify potential in AIM-listed shares with a market capitalization below £10 million. Specifically, it focuses on stocks that have shown significant downside and minimal upside price movement, defined as decreasing by more than 65% and increasing by less than 15% from their closing price 9 months ago. The intent is to screen for companies that may be in a full-on downtrend or have bottomed out.

Screening for significant decline is essential because it helps investors identify shares that are experiencing strong negative momentum. Such stocks often reflect underlying factors like deteriorating financial performance, unsuccessful business strategies, or decreased market interest. By identifying these declining opportunities early, investors can capitalize on the downward trends for potentially substantial returns through short selling. Furthermore, understanding these trends can also present opportunities to buy stocks at a lower price if a potential recovery is anticipated.

## Setup

### Choose Your Environment
You can run this project either locally using Jupyter Lab or online using Google Colab. Follow the appropriate setup instructions below:

### Running the Notebook Locally with Jupyter Lab

1. **Install Jupyter Lab**:
   - Open your command line (Terminal on macOS/Linux or Command Prompt on Windows).
   - Install Jupyter Lab using pip:
     ```sh
     pip install jupyterlab
     ```

2. **Download the Project**:
   - Download the project files from the repository. You can download it as a ZIP file from GitHub and extract it to your desired directory.
   - Alternatively, you can clone the repository using Git:
     ```sh
     git clone https://github.com/your-username/project-repo.git
     cd project-repo
     ```

3. **Start Jupyter Lab**:
   - Navigate to the project directory in your command line:
     ```sh
     cd path/to/your/project/directory
     ```
   - Start Jupyter Lab:
     ```sh
     jupyter lab
     ```

4. **Open Jupyter Lab**:
   - Your default web browser will open Jupyter Lab, typically at `http://localhost:8888/lab`.

5. **Upload Files (if necessary)**:
   - In the Jupyter Lab interface, you can upload files by clicking the "Upload" button in the file browser pane on the left. Select the files you need from your local machine.

6. **Open the Notebook**:
   - In the Jupyter Lab interface, navigate to the project directory.
   - Open the `[notebook file]` notebook file.

### Running the Notebook Online with Google Colab

1. **Open Google Colab**:
   - Go to [Google Colab](https://colab.research.google.com/).

2. **Upload the Notebook**:
   - Click on `File` > `Upload notebook` and select the `[notebook file]` file you downloaded.

## Running the Project

Once you have chosen your environment (Jupyter Lab or Google Colab) and set it up, follow these steps to run the project:

### Run the Notebook Cells

Execute each cell in the notebook sequentially to collect the data, define the thresholds, and display results.

The project comes with a notebook named `aim_casino_ticker_collect.ipynb` which creates `aim_ticker_list.csv`. This CSV file is included in the project, so running the notebook is optional.

To perform the main analysis, run the notebook named `aim_casino_screener_significant_decline.ipynb`.

Running the following code snippet in the project will create `aim_analysis.csv`:

for symbol in tqdm(df_loaded.index, desc='Fetching Stock Data', unit='symbol'):

However, `aim_analysis.csv` is already included in the project. Therefore, you can skip the data downloading step and jump directly to the "Define the threshold percentages" section to continue with the analysis.

## Acknowledgments
Thank you to everyone who supported and contributed to this project.

## License
This project is licensed under the MIT License.
