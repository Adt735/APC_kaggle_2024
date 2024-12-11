# APC_kaggle_2024
This repository has all the necessary to get the dataset, analyse it, train regression models and evaluate its performance.

# Use
## 01: Get the dataset
* Given a `.png` file and the Stockfish engine installed on your computer, this jupyter notebook has all the necessary functions to create a dataset filled with the FENs of the games and the Stockfish evaluation.
  This dataset is already in the GitHub, it's called `dataset_.csv`
* If you'd like to train use the other notebooks, you must process the dataset obtained using this notebook with the chess engine from: https://github.com/Adt735/linear_chess_engine

## 02: EDA
* This ipynb has only basics visualization of the correlation between the variables and the Stockfish evaluation.

## 03: Training
This notebook has multiple parts, all using the dataset obtained with the first notebook
1. Perform first predictions with default values
2. Search the best hyperparameters. The result is stored in the GitHub. It's the `hyperparameters_search_results.csv` file
3. Train the best model with all the data and save the coefficients to a file. There's currently 3 files with valid coefficients that can be used with the linear_chess_engine. The `linear_model.json` is the direct result of the best model, and the `coefficients.json` file has the from the ChessProgramming page.

## 04: Use the model
* To use the model, just download the chess engine from https://github.com/Adt735/linear_chess_engine and follow the instructions.
* There's a folder in this repo with some matches of different models playing against each other.

