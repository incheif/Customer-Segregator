# **Customer Segmentation with Machine Learning**

### **Project Overview**
This project aims to segment customers into different groups based on their purchasing behavior and demographics using unsupervised learning techniques. Customer segmentation helps businesses understand their target audience better, enabling them to tailor marketing strategies, improve product offerings, and optimize customer experiences.

### **Key Features**
- Implements **K-Means Clustering** to group customers based on their **Age**, **Annual Income**, and **Spending Score**.
- Uses **Elbow Method** to find the optimal number of clusters.
- Visualizes the clusters to interpret customer segments clearly.
- Provides **insights** about different customer groups and how businesses can target them.

### **Technologies Used**
- **Python**: Core language used for data analysis and machine learning.
- **Pandas**: Data manipulation and analysis.
- **Scikit-learn**: Machine learning algorithms, including K-Means clustering.
- **Matplotlib & Seaborn**: Data visualization libraries.
- **NumPy**: Numerical computing for efficient calculations.

### **Project Structure**
```bash
.
├── dataset/
│   └── Mall_Customers.csv     # The dataset used for customer segmentation.
├── src/
│   └── customer_segmentation.ipynb  # Jupyter Notebook with the code for analysis and clustering.
└── README.md                  # This file with project details and instructions.
```

### **Dataset**
The dataset used is the **Mall Customer Segmentation Data**, which contains the following features:
- **CustomerID**: Unique identifier for each customer (not used in analysis).
- **Gender**: Gender of the customer (Male = 0, Female = 1).
- **Age**: Age of the customer.
- **Annual Income (k$)**: The customer’s annual income (in thousands of dollars).
- **Spending Score (1-100)**: A score assigned by the mall based on the customer’s behavior and spending nature.

### **How to Run the Project**
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/customer-segmentation-ml.git
   cd customer-segmentation-ml
   ```

2. **Install Dependencies**:
   Ensure you have Python 3.x installed and install the necessary libraries using:
   ```bash
   pip install -r requirements.txt
   ```

   The `requirements.txt` should contain:
   ```
   pandas
   numpy
   scikit-learn
   matplotlib
   seaborn
   ```

3. **Run the Jupyter Notebook**:
   Open the Jupyter notebook to explore the code and execute each step.
   ```bash
   jupyter notebook src/customer_segmentation.ipynb
   ```

4. **View the Dataset**:
   The dataset (`Mall_Customers.csv`) should be placed inside the `dataset/` directory. You can also load your own dataset by modifying the path in the code.

### **Steps in the Project**
1. **Data Preprocessing**:
   - Load the dataset and clean it by handling missing values and encoding categorical variables.
   - Standardize the numerical features for clustering.

2. **Clustering**:
   - Apply the **Elbow Method** to determine the optimal number of clusters.
   - Perform **K-Means Clustering** using the optimal number of clusters.

3. **Visualization**:
   - Visualize the customer segments using scatter plots and 3D plots.
   - Analyze the different customer segments based on **Age**, **Annual Income**, and **Spending Score**.

4. **Cluster Analysis**:
   - Derive business insights for each customer group (e.g., premium customers, discount-seekers, value buyers).

### **Results**
- After performing clustering, customers were segmented into distinct groups based on their spending behavior and demographics.
- These segments can be used to create targeted marketing campaigns, offer personalized services, or optimize product recommendations for each customer group.

### **Business Insights**
- **High-income, high-spending customers**: Can be targeted with premium products and exclusive offers.
- **Young, low-income, high-spending customers**: Likely respond to discounts and affordable trendy products.
- **Older, low-spending customers**: May prefer practical, value-for-money offerings.

### **Future Enhancements**
- Implement **DBSCAN** for comparison with K-Means.
- Use more features (e.g., purchase frequency, product categories) for richer segmentation.
- Experiment with **deep learning** methods such as Autoencoders for advanced clustering.

### **Contributing**
If you have any suggestions or improvements, feel free to fork the repository and submit a pull request!

### **License**
This project is licensed under the MIT License.
