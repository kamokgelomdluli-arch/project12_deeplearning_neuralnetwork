# project12_deeplearning_neuralnetwork


# Used Car Price Prediction (PyTorch)

A neural network that predicts the price of a used car from its listing details.

## What It Does

It is a regression model. It takes used car listing data and predicts the sale price.

## packages used

- **PyTorch** — built the network and handled training
- **Pandas** — loaded and cleaned the data
- **Scikit-learn** — split and scaled the data
- **Matplotlib** — visualized data

## What i Did

1. Loaded 20,000 rows of used car data
2. Cleaned it — dropped rows with missing values, converted `cylinders` to numbers, dropped the `state` column
3. Encoded text columns as one-hot vectors (112 features)
4. Split into train / dev / test (80 / 10 / 10)
5. Scaled features and the target (`price`) separately with `StandardScaler`
6. Built a 4-layer network: input → 100 ReLU → 100 ReLU → 25 ReLU → 1 linear
7. Trained for 1,000 epochs with SGD (lr = 0.2) and MSE loss
8. Evaluated and plotted predictions vs. true values



