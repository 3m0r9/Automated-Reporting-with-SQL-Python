
📊 Automated Reporting with SQL & Python

This project demonstrates how to automate the process of querying data from a SQL database, generating reports using Python, and exporting the results into structured Excel files. It is particularly useful for business analysts, data engineers, or teams that require daily/weekly automated reports.

---

## 🚀 Features

- ✅ Connects to a SQL Server database using `pyodbc`
- ✅ Executes parameterized SQL queries
- ✅ Automates daily or scheduled report generation
- ✅ Exports results to Excel (.xlsx) with formatted sheets
- ✅ Handles exceptions and logging for reliability

---

## 🛠️ Tech Stack

- **Language**: Python 3.x  
- **Database**: Microsoft SQL Server  
- **Libraries Used**:
  - `pandas`
  - `pyodbc`
  - `openpyxl`
  - `os`, `datetime`, `time`

---

## 📁 Project Structure

```

Automated-Reporting-with-SQL-Python/
├── sql\_query.sql           # Contains the SQL query for the report
├── config.py               # Configuration (DB credentials, file paths)
├── report\_generator.py     # Main script to run the automation
├── requirements.txt        # Required libraries
└── README.md               # Project documentation

````

---

## ⚙️ How It Works

1. **Connect to the Database**:  
   `pyodbc` establishes a secure connection to the SQL Server using credentials in `config.py`.

2. **Run SQL Query**:  
   The script reads a `.sql` file and executes it dynamically.

3. **Generate Report**:  
   Results are loaded into a pandas DataFrame and written to Excel using `openpyxl`.

4. **Automation Ready**:  
   You can schedule this script using Task Scheduler (Windows) or `cron` (Linux/macOS) for regular execution.

---

## 📦 Setup Instructions

1. **Clone the Repo**  
   ```bash
   git clone https://github.com/3m0r9/Automated-Reporting-with-SQL-Python.git
   cd Automated-Reporting-with-SQL-Python
````

2. **Install Dependencies**

   ```bash
   pip install -r requirements.txt
   ```

3. **Edit `config.py`**
   Add your database credentials and output directory.

4. **Run the Script**

   ```bash
   python report_generator.py
   ```

---

## 📅 Use Case Example

* A retail company wants to send **daily sales summaries** to regional managers.
* This tool runs at 6:00 AM every day and generates Excel reports from their database.
* The report is emailed via a separate integration (can be extended).

---

## ✍️ Author

* **Imran Abu Libda**

- **GitHub** - [3m0r9](https://github.com/3m0r9)
- **LinkedIn** - [Imran Abu Libda](https://www.linkedin.com/in/imran-abu-libda/)
- **Email** - [imranabulibda@gmail.com](mailto:imranabulibda@gmail.com)
- **Medium** - [Imran Abu Libda](https://medium.com/@imranabulibda_23845)

---

## 📄 License

This project is licensed under the MIT License – see the [LICENSE](LICENSE) file for details.

---

## 🙌 Contributions

Pull requests and feedback are welcome. For major changes, please open an issue first to discuss what you would like to change.
