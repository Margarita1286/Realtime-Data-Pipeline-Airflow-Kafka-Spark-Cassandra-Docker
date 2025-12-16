# 🚀 How to Run the Project (Next Time)

Here are the instructions for running both versions of your application.

---

## 🟢 Option 1: Run Cloud/Demo Version (Easiest)
*Use this for quick demos, UI checks, or if you don't want to turn on Docker.*

1.  **Open Terminal** in your project folder:
    ```bash
    cd "C:\Users\rattu\Downloads\P-6"
    ```
2.  **Run Streamlit**:
    ```bash
    streamlit run streamlit_app.py
    ```
    *(Note: This runs the simulator version we moved to the root folder)*

---

## 🔴 Option 2: Run Full Local System (Real)
*Use this when you want to process actual data, check Kafka topics, or work on the backend.*

1.  **Open Terminal** in the backend folder:
    ```bash
    cd "C:\Users\rattu\Downloads\P-6\airflow-kafka-spark-cassandra-streaming"
    ```

2.  **Start Docker Containers**:
    ```bash
    docker-compose up -d
    ```
    *⏳ Wait about 3-5 minutes for Cassandra and Kafka to fully start up.*

3.  **Check Containers are Running**:
    ```bash
    docker ps
    ```

4.  **Run the Streamlit App**:
    ```bash
    streamlit run streamlit_app.py
    ```

### 🛑 Stopping Everything
When you are done with Option 2, always clean up to save RAM:
```bash
docker-compose down
```
