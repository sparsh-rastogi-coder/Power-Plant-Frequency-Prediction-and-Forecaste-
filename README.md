# **Power Plant Frequency Forecast**  
Harnessing the power of **Machine Learning** and **Deep Learning**, this project predicts power grid frequency variations using an **ARIMA-LSTM Hybrid Model** to ensure accuracy and reliability in time series forecasting.  

---

## **🔹 ARIMA-LSTM Hybrid Model: A Synergistic Approach**  

This project integrates:  
✅ **ARIMA (AutoRegressive Integrated Moving Average)** – Captures linear trends and seasonality.  
✅ **LSTM (Long Short-Term Memory)** – Learns complex nonlinear dependencies in time series data.  
🔄 **Hybrid Approach** – ARIMA models the linear component, while LSTM captures residual nonlinear patterns, leading to improved predictive accuracy.  

---

## **📌 Data Processing: From Raw PDFs to Structured Insights**  

### **1️⃣ Data Extraction**  
📄 **Source:** Frequency profile reports in PDF format.  
🛠 **Processing Script:** `pdf_to_csv_with_proper_heading.py` extracts and structures the data.  

✔ **Steps Involved:**  
- Extracts text using `pdfplumber`.  
- Parses data to identify **column headers (days) & time blocks (frequency values)**.  
- Converts extracted data into a structured **CSV file** with a well-organized format.  

### **2️⃣ Data Transformation & Merging**  
📂 **Script Used:** `transposedata.py` processes each monthly CSV from `transformed_data2024/`.  
📊 **Key Processing Steps:**  
- Reformats dates into **DD-MM-YYYY** format.  
- Merges all monthly CSVs into a **final dataset**: `maha_data.csv`.  

---

## **⚙️ Dependencies**  

Ensure you have the required Python packages installed:  
```bash
pip install numpy pandas matplotlib scikit-learn statsmodels tensorflow keras pdfplumber
```

---

## **🚀 Running the Model**  

1️⃣ **Clone the repository** or download the notebook.  
2️⃣ **Install dependencies** (see above).  
3️⃣ **Open the notebook** using:  
   ```bash
   jupyter notebook arima_lstm.ipynb
   ```
4️⃣ **Run all cells sequentially** to:  
   - Preprocess data  
   - Train the hybrid model  
   - Visualize forecasting results  

---

## **📈 Model Performance & Results**  

The model is evaluated using key error metrics:  
📉 **RMSE (Root Mean Squared Error)**  
📉 **MAE (Mean Absolute Error)**  

📊 **Graphical analysis** further validates the forecast accuracy.  

---

## **🔮 Future Enhancements**  

🚀 **Hyperparameter tuning** for improved performance.  
📅 **Forecasting at a monthly scale** for extended time horizons.  
📡 **Testing on larger and more complex datasets**.  
🔬 **Exploring advanced hybrid models** like **LSTM+CNN** for enhanced precision.  

---

This project demonstrates the power of blending **statistical** and **deep learning** approaches to time series forecasting, paving the way for more accurate power grid frequency predictions. ⚡📊

