# Multi-Model Data Fusion with MNIST Images

This project demonstrates multi-model data fusion by combining synthetic customer data, purchase history, website activity, and image data from the MNIST dataset. The goal is to create a comprehensive dataset that offers a richer and more complete view of the information.

## Overview

Multi-model data fusion involves merging data from different sources to provide a holistic view of the data. In this project, we fuse:

1. Customer Data: Basic information about customers.
2. Purchase Data: Customers' purchase history.
3. Website Activity Data: Customers' activities on a website.
4. MNIST Image Data: Handwritten digit images.

## Data Sources

### 1. Customer Data

This dataset includes basic customer information such as:
- Customer ID
- Name
- Age
- Email

### 2. Purchase Data

This dataset records customers' purchase history, including:
- Purchase ID
- Customer ID
- Product
- Amount

### 3. Website Activity Data

This dataset logs customers' activities on a website, including:
- Activity ID
- Customer ID
- Page Visited
- Duration

### 4. MNIST Image Data

The MNIST dataset consists of handwritten digit images. For this example, we use a small subset of these images.

## Steps Involved

1. **Data Collection**:
   - Generate synthetic data for customer information, purchase history, and website activity.
   - Download a small subset of the MNIST dataset to reduce time and memory usage.

2. **Data Preparation**:
   - Ensure each dataset contains a common identifier (customer ID) to enable merging.
   - Preprocess the image data to associate it with the corresponding customer IDs.

3. **Data Fusion**:
   - Merge the customer data with the purchase data using the customer ID.
   - Merge the resulting dataset with the website activity data.
   - Finally, merge the combined dataset with the MNIST image data.

4. **Output**:
   - Display and save the fused dataset, which now contains a comprehensive view of each customer, including their basic information, purchase history, website activity, and associated image data.

## Project Structure

```
.
├── mnist_data
│   ├── <MNIST data files>
├── multi_model_fused_data.csv
├── README.md
└── data_fusion_notebook.ipynb
```

## Usage

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/multi-model-data-fusion.git
   cd multi-model-data-fusion
   ```

2. **Install the required libraries**:
   ```bash
   pip install pandas numpy matplotlib scikit-learn tqdm
   ```

3. **Run the Jupyter Notebook**:
   ```bash
   jupyter notebook data_fusion_notebook.ipynb
   ```

## Display Sample Images

The notebook includes functionality to display a small sample of the MNIST images to be fused, providing visual confirmation of the images being included in the data fusion process.

## Save Fused Data

The fused data is saved to a CSV file named `multi_model_fused_data.csv`, excluding the image data for simplicity.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License.

## Acknowledgements

- The MNIST dataset is provided by Yann LeCun and Corinna Cortes.
- This project utilizes `pandas`, `numpy`, `matplotlib`, `scikit-learn`, and `tqdm`.
