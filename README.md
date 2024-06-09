---

## Project Title: Personalized Product Recommendation System

## Project Description

This project aims to build a Personalized Product Recommendation System to enhance user experience by providing tailored product suggestions. By employing Apache Spark for scalable data processing and utilizing collaborative filtering and product-based recommendation algorithms, the system efficiently handles large datasets and delivers accurate recommendations.

## Features

- **Scalable Data Processing**: Leveraged Apache Spark for rapid and scalable analysis of large datasets, particularly product reviews.
- **Collaborative Filtering**: Implemented collaborative filtering using matrix decomposition techniques to recommend products based on user behavior.
- **Product-Based Recommendation**: Developed a product-based recommendation model using clustering algorithms to group similar products and provide relevant suggestions.
- **Evaluation Metrics**: Assessed the performance of the recommendation models using metrics like RMSE and precision-recall.

## Technologies Used

- **Programming Languages**: Python, Scala
- **Big Data Framework**: Apache Spark
- **Machine Learning Libraries**: Scikit-learn, Spark MLlib
- **Data Processing Libraries**: Pandas, NumPy
- **Visualization**: Matplotlib, Seaborn
- **Deployment**: Flask, Docker

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/product-recommendation-system.git
   ```
2. Navigate to the project directory:
   ```bash
   cd product-recommendation-system
   ```
3. Create a virtual environment:
   ```bash
   python3 -m venv venv
   ```
4. Activate the virtual environment:
   - On Windows:
     ```bash
     venv\Scripts\activate
     ```
   - On macOS/Linux:
     ```bash
     source venv/bin/activate
     ```
5. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage

1. **Data Preprocessing**:
   - Place your product reviews and user interaction data in the `data/` directory.
   - Run the data preprocessing script to clean and prepare the data:
     ```bash
     python preprocess_data.py
     ```

2. **Model Training**:
   - Train the collaborative filtering model:
     ```bash
     python train_collaborative_filtering.py
     ```
   - Train the product-based recommendation model:
     ```bash
     python train_product_based.py
     ```

3. **Model Evaluation**:
   - Evaluate the performance of the trained models:
     ```bash
     python evaluate_models.py
     ```

4. **Model Deployment**:
   - Start the Flask web application to serve the recommendation models:
     ```bash
     python app.py
     ```

5. **Visualization Dashboard**:
   - Access the interactive dashboard by navigating to `http://localhost:5000` in your web browser.

## Project Structure

```
product-recommendation-system/
│
├── data/
│   └── reviews.csv
│   └── user_interactions.csv
│
├── models/
│   ├── collaborative_filtering_model.pkl
│   └── product_based_model.pkl
│
├── notebooks/
│   └── exploratory_data_analysis.ipynb
│
├── scripts/
│   ├── preprocess_data.py
│   ├── train_collaborative_filtering.py
│   ├── train_product_based.py
│   ├── evaluate_models.py
│   └── app.py
│
├── templates/
│   └── index.html
│
├── requirements.txt
├── README.md
└── Dockerfile
```

## Key Scripts

- **preprocess_data.py**: Handles data cleaning and preparation for model training.
- **train_collaborative_filtering.py**: Builds and trains the collaborative filtering model using matrix decomposition techniques.
- **train_product_based.py**: Develops and trains the product-based recommendation model using clustering algorithms.
- **evaluate_models.py**: Evaluates the models' performance using metrics like RMSE and precision-recall.
- **app.py**: Flask application script for serving the recommendation models and displaying the dashboard.

## Visualization

- **User-Product Interaction Matrix**: Visualization of the user-product interaction matrix used in collaborative filtering.
- **Product Clusters**: Visual representation of product clusters formed during the product-based recommendation.
- **Evaluation Metrics**: Graphs showing the evaluation metrics for model performance.

## Deployment with Docker

1. Build the Docker image:
   ```bash
   docker build -t product-recommendation-system .
   ```
2. Run the Docker container:
   ```bash
   docker run -p 5000:5000 product-recommendation-system
   ```

## Contributors

- Harshal Dhandrut - [GitHub](https://github.com/harshal-96)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---
