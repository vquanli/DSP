# DSP
The rainfall evaluation model based on XGBoost.

## Project Objective

The primary objective of is to bridge the trust gap between farmers and insurance providers, reduce operational costs, and expedite claims settlement, ensuring a more reliable and efficient agricultural insurance system.

## Key Features

- **Rainfall Estimation using Machine Learning**: Utilizes XGBoost's Gradient Boosted Decision Trees classifier for accurate prediction of rainfall.
- **Refined Prediction Mechanism**: Enhances predictions using meteorological base station data.
- **Zero-Knowledge Proofs**: Ensures data integrity and privacy by validating model predictions without revealing underlying data.
- **Decentralized System**: Transfers loss assessment from insurance companies to a transparent, decentralized system.

## Data

The project uses data from the "How Much Did It Rain?" competition on Kaggle, including NEXRAD and MADIS data in CSV format, with over a million samples for training and over 600,000 for testing.

## Installation

1. Clone the repository.
2. Install required Python packages.
3. Prepare data
Download [data](https://www.kaggle.com/competitions/how-much-did-it-rain/data). Place the `train_2013.csv` and `test_2014.csv` files into the `input` folder. 

## Usage

Model generation and prediction (Roughly 10 hours):
Navigate to the `code` directory:
```
cd Rain_Forust/code
./main.sh
```
  Once in the `code` folder, execute the script by typing `./main.sh`. Ensure that the following folders are present at the top level of the directory: `input`, `code`, `processed`, `models`, and `output`.


## Dependencies

- Python 3.x
- XGBoost
- Pandas
- NumPy
- forust
- RISC Zero's zkVM (for zero-knowledge proof validation)

## Contributing

Contributions are welcome. Please fork the repository and submit a pull request with your proposed changes.


## Contact

For any queries or contributions, please feel free to contact.

## Acknowledgments

- Kaggle's "How Much Did It Rain?" competition data
- Rain_Forus builds on the Devin Anzelmo [model](https://www.kaggle.com/competitions/how-much-did-it-rain/discussion/14860) and extends the forust-based approach to model training and prediction.

---
