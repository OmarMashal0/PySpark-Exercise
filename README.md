# 🚀 PySpark Exercises & Tasks

A collection of **hands-on PySpark exercises with solutions** to practice **big data processing** using Apache Spark.  

---

## 📌 What’s Inside
- **RDD Operations** → transformations, actions, grouping, aggregations.  
- **DataFrames & SQL** → filtering, grouping, distinct counts, average salary.  
- **Joins & Preprocessing** → handle missing values, replace nulls, clean data.  
- **Text Processing** → word count, stopwords removal, top frequent words.  
- **File Handling** → read/write CSV & JSON.  

Datasets included:  
- `NullData.csv` → sample sales data with nulls.  
- `russia.txt` → text file for word count.  

---

## 🐳 Running with Docker
1. **Clone the repo**  
   ```bash
   git clone https://github.com/OmarMashal0/PySpark-Exercise.git
   cd PySpark-Exercise
   ```
2. **Start the cluster**  
   ```bash
   docker compose -f depi.yaml up -d
   ```
   Containers: Spark master, Spark worker, HDFS (namenode + datanode), Jupyter Notebook.  
3. **Access services**  
   - 📓 Jupyter → [http://localhost:8888](http://localhost:8888)  
   - 📊 Spark UI → [http://localhost:4040](http://localhost:4040)  
4. **Stop cluster**  
   ```bash
   docker compose -f depi.yaml down
   ```
   
---

## 📊 Example Outputs
**Average Salary**  
```
+----------+
|avg_salary|
+----------+
|    6000.0|
+----------+
```

** Group by a the name column and find average salary **  
```
+------+----------+
|  name|avg_salary|
+------+----------+
|   Ali|    4000.0|
|Mariam|    6750.0|
|  Omar|    6750.0|
|  Sara|    5000.0|
+------+----------+
```
