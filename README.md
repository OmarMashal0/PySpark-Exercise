# 🚀 PySpark Exercises & Tasks

A collection of **hands-on PySpark exercises with solutions** to practice **big data processing** using Apache Spark.  
Perfect for **students, data engineers, and interview prep**.

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

## 📘 How to Use
- Open exercises in **Jupyter Notebook** (`Task.ipynb`) and solve them.  
- Compare with provided **solutions**.  
- Run standalone `.py` scripts with Spark Submit:  
  ```bash
  docker exec -it pyspark-container spark-submit scripts/example.py
  ```

---

## 📊 Example Outputs
**Average Salary**  
```
6000.0
```

**Filter Employees Older than 28**  
```
+---+------+---+------+
| id|  name|age|salary|
+---+------+---+------+
|  2|Mariam| 30|  6000|
|  3|  Omar| 35|  7000|
+---+------+---+------+
```

---

## 🤝 Contributing
Contributions welcome 🎉  
1. Fork → Branch → Commit → PR.  
