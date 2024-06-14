Histology Diagnosis Extraction with Transformers

This project focuses on extracting histology diagnosis from text reports using a transformer-based model. The code preprocesses text files, tokenizes the content, creates a dataset, and uses a pre-trained language model to generate the diagnosis.

Table of Contents
Installation
Usage
Project Structure
Contributing
License
Installation
To run this project, you need to install the following dependencies:

bash
Copy code
pip install torch transformers accelerate pandas pyreadr
Ensure you have a compatible GPU setup for optimal performance.

Usage
Prepare Your Data: Place your text reports in the under_run_samples directory.

Run the Code: Execute the provided script to preprocess the data, create batches, and generate histology diagnoses.

python
Copy code
python main.py
Project Structure
main.py: The main script that includes data preprocessing, dataset creation, and model inference.
under_run_samples/: Directory containing the text reports to be analyzed.
Script Overview
Imports and Parameters: Import necessary libraries and set up parameters.
Device Setup: Configure device for CUDA if available.
Data Preparation: Preprocess text files and tokenize the content.
Custom Dataset Class: Define a custom dataset class to handle data loading.
Data Loader: Create a DataLoader for batching.
Model Inference: Load the pre-trained model and generate histology diagnoses.
Example
Here is a simplified example of how to use the script:

python
Copy code
# Set the path to your model and sample data
model_id = "path_to_your_model"
sample_folder_path = "./under_run_samples"

# Ensure your text reports are in the specified directory
# Run the script to see the output
python main.py
Contributing
Contributions are welcome! Please feel free to submit a Pull Request or open an issue for any bugs or feature requests.

License
This project is licensed under the MIT License. See the LICENSE file for details.
