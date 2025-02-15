# Customer Segmentation Using RFM and K-Means

## 📌 Project Overview  
This project applies **RFM (Recency, Frequency, Monetary) analysis** and **K-Means Clustering** to segment customers based on their purchasing behavior. The goal is to identify different customer groups and provide actionable insights for businesses to improve **customer retention, loyalty, and marketing strategies**.

## 📂 Dataset  
The dataset used in this project is the **Online Retail Dataset**, which contains **customer transactions over two years**.  
Key columns include:  
- `InvoiceNo` - Unique identifier for each transaction  
- `Quantity` - Number of items purchased  
- `Price` - Unit price of the product  
- `CustomerID` - Unique identifier for each customer  
- `TotalPrice` - Computed as `Quantity × Price`  

## ⚙️ Steps in the Project  

### **1. Data Preprocessing**  
- Removed missing `CustomerID` values and negative `Quantity` values  
- Converted `InvoiceDate` to a proper datetime format  
- Computed `TotalPrice` for each transaction  

### **2. RFM Analysis**  
- **Recency (R):** Days since the last purchase  
- **Frequency (F):** Number of unique purchases made  
- **Monetary (M):** Total spending of the customer  
- Applied **log transformation** and **scaling** to normalize data  

### **3. K-Means Clustering**  
- Used the **Elbow Method** to determine the optimal number of clusters (K=4)  
- Performed **clustering** and labeled customers into **four groups:**  
  - **High Value Customers**  
  - **Moderate Value Customers**  
  - **Low Value Customers**  
  - **Recent Buyers**  

### **4. Data Visualization & Insights**  
#### ✅ **Pie Chart: Cluster Distribution**  
- Displays the proportion of customers in each segment.  

#### ✅ **Scatter Plot: Recency vs Monetary**  
- **High-Value customers (Red):** Bought recently and spent the most.  
- **Low-Value customers (Purple):** Haven't purchased in a long time and spent less.  

#### ✅ **Scatter Plot: Frequency vs Monetary**  
- **Frequent buyers in the High-Value cluster (Red)** tend to have **higher spending**.  
- **Recent Buyers (Blue)** have **low frequency and spending** since they are **new customers**.  

## 🛠️ Technologies Used  
- **Python**  
- **Pandas**  
- **NumPy**  
- **Matplotlib & Seaborn** (for visualization)  
- **Scikit-learn** (for clustering and preprocessing)  

## 📌 Key Takeaways  
- **Segmenting customers** helps businesses **personalize marketing strategies**.  
- **High-value customers** can be targeted with loyalty programs.  
- **Low-value customers** might need engagement strategies to boost purchases.  

## 🚀 How to Run the Project  
1. Clone the repository:  
   ```bash
   git clone https://github.com/Daniyal-DS/Customer-Segmentation-Using-RFM-and-KMeans
📌 Author
👤 Daniyal Haider
💼 LinkedIn Profile https://www.linkedin.com/in/daniyal-haider-74a63a201/
📧 haiderdaniyal095@gmail.com
