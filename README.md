# MLP-house-pricing
# House Price Prediction Using Simple Neural Network (MLP)

## Project Overview

The goal of this project is to **predict house prices** using a **simple neural network (Multi-Layer Perceptron, MLP)**.  
We use numerical and categorical features of houses to train the model and predict prices accurately. The network employs the **ReLU activation function** in hidden layers to capture non-linear relationships between features and target prices.

## Neural Network & Activation Function

### Neural Network (MLP)
A **neural network** is a computational model inspired by the human brain, composed of **layers of interconnected nodes (neurons)**. Each neuron processes input data and passes it through an activation function to the next layer.  

**MLP (Multi-Layer Perceptron)** is a type of feedforward neural network with one or more hidden layers. It can approximate complex, non-linear functions, making it suitable for regression tasks like house price prediction.

### Activation Function: ReLU
The **ReLU (Rectified Linear Unit)** function is defined as:
ReLU(x) = max(0, x)

- ReLU introduces **non-linearity** to the network, allowing it to model complex patterns.  
- It is computationally efficient and helps avoid the vanishing gradient problem in deep networks.

## Dataset Features

The dataset contains detailed information about each property. Some of the key features include:

- **MSSubClass**: Type of dwelling involved in the sale (e.g., 1-STORY 1946 & NEWER, 2-STORY, Duplex, etc.).  
- **MSZoning**: General zoning classification (e.g., Residential Low Density, Commercial, Agriculture).  
- **LotFrontage**: Linear feet of street connected to property.  
- **LotArea**: Lot size in square feet.  
- **Street**: Type of road access (Gravel or Paved).  
- **Alley**: Type of alley access (Gravel, Paved, or None).  
- **LotShape**: General shape of property (Regular, Slightly Irregular, etc.).  
- **LandContour**: Flatness of property (Level, Hillside, Banked, etc.).  
- **Utilities**: Type of utilities available (All public utilities, electricity & gas only, etc.).  
- **LotConfig**: Lot configuration (Inside, Corner, Cul-de-sac, etc.).  
- **Neighborhood**: Physical location within the city.  
- **OverallQual**: Overall material and finish quality (1-10 scale).  
- **OverallCond**: Overall condition (1-10 scale).  
- **YearBuilt**: Original construction year.  
- **YearRemodAdd**: Remodel year.  
- **RoofStyle**, **RoofMatl**, **Exterior1st**, **Exterior2nd**, **MasVnrType**, **MasVnrArea**, **ExterQual**, **ExterCond**: Building materials and quality.  
- **Foundation**, **BsmtQual**, **BsmtCond**, **BsmtExposure**, **BsmtFinType1**, **BsmtFinType2**, **BsmtFinSF1**, **BsmtFinSF2**, **BsmtUnfSF**, **TotalBsmtSF**: Basement features and areas.  
- **Heating**, **HeatingQC**, **CentralAir**, **Electrical**: Utilities and HVAC features.  
- **1stFlrSF**, **2ndFlrSF**, **LowQualFinSF**, **GrLivArea**: Living area features.  
- **FullBath**, **HalfBath**, **BsmtFullBath**, **BsmtHalfBath**, **Bedroom**, **Kitchen**, **KitchenQual**, **TotRmsAbvGrd**: Room and bathroom counts & quality.  
- **Fireplaces**, **FireplaceQu**: Fireplace features.  
- **GarageType**, **GarageYrBlt**, **GarageFinish**, **GarageCars**, **GarageArea**, **GarageQual**, **GarageCond**: Garage features.  
- **PavedDrive**, **WoodDeckSF**, **OpenPorchSF**, **EnclosedPorch**, **3SsnPorch**, **ScreenPorch**, **PoolArea**, **PoolQC**, **Fence**, **MiscFeature**, **MiscVal**: Outdoor and miscellaneous features.  
- **MoSold**, **YrSold**, **SaleType**, **SaleCondition**: Sale information.

> The dataset contains both **numerical and categorical features**, which are preprocessed before feeding into the neural network.

## Methodology

1. **Data Preprocessing**  
   - Handle missing values  
   - Encode categorical variables  
   - Normalize numerical features  

2. **Model Construction**  
   - Define a simple MLP with input, hidden, and output layers  
   - Use **ReLU activation** in hidden layers  

3. **Training**  
   - Split dataset into training and testing sets  
   - Train the network using backpropagation and optimize loss  

4. **Prediction & Evaluation**  
   - Predict house prices on test data  
   - Evaluate model performance using metrics such as **MSE** and **R² score**  
