
# Analyzing Cryptocurrency Market Trends: Unveiling Patterns and Predicting the Future

## Setup Instructions

### 1. Download the Dataset
1. Go to [CoinMarketCap Bitcoin Data](https://coinmarketcap.com/currencies/bitcoin/).
2. Next to the buttons where you can choose time ranges like 1D, 7D, 1M, etc., there will be three dots (`...`) as a dropdown menu.
3. Select this dropdown, and you will see the option to download the data as a CSV file.
4. Save the CSV file to your local system for use in the project.

**There is a sample csv file attached within this repo, called: BTC_7D_graph_coinmarketcap.csv**

---

### 2. Creating the Virtual Environment
To isolate project dependencies, create a virtual environment:

```bash
python -m venv venv
```

---

### 3. Activating the Virtual Environment
Activate the virtual environment with the following command:

- **Linux/Mac**:
  ```bash
  source ./venv/bin/activate
  ```

- **Windows**:
  ```bash
  .\venv\Scripts\activate
  ```

---

### 4. Installing Required Libraries
Install all necessary libraries by running:

```bash
pip install -r requirements.txt
```

---

### 5. Configuring the Python Code
To properly run the project, you need to make the following updates in the Python code:

1. **MySQL Configuration**: Provide the correct host, username, and password in the `db_config` dictionary to successfully connect to your MySQL database.
   ```python
   db_config = {
       'host': 'your_mysql_host',
       'user': 'your_mysql_username',
       'password': 'your_mysql_password',
       'database': 'your_database_name'
   }
   ```

2. **File Path for CSV**: Update the `csv_file` variable in the `create_database_and_table` function to the location where you saved the CSV file.
   ```python
   csv_file = "path_to_your_downloaded_csv_file.csv"
   ```

---

### 6. Running Jupyter Notebook
Follow these steps to open and execute the project notebook:

1. Start the Jupyter Notebook server by running:
   ```bash
   jupyter notebook
   ```

2. Once the server starts, a browser window will open showing the file directory.

3. Navigate to the project folder and open the **`crypto.ipynb`** file.

4. Execute the notebook cell by cell to process the data and evaluate the model.

---

### Demo Video

Within the codebench submission, there is code that can be run to launch the video within Jupyter Notebook. 
Alternatively, you can access the demo video using this link:

https://drive.google.com/file/d/16ufPBbf2Oys-NEXPNZvsLz4UPN5W9BMi/view?usp=sharing

---

### Repository Structure
- **`crypto.ipynb`**: The main Jupyter Notebook for analyzing and visualizing cryptocurrency data.
- **`requirements.txt`**: Contains all the necessary dependencies for this project.
- **`README.md`**: Instructions and documentation for setting up and running the project.
- **`BTC_7D_graph_coinmarketcap.csv`**: Sample csv file for testing.

---
