# Travel Purpose Prediction with Machine Learning
This project aims to predict the purpose of a user's travel booking—whether it's for work or leisure—using data from travel bookings on the Mr. Bilit website. The model leverages XGBoost, a highly efficient gradient boosting algorithm, to classify travel bookings based on various features, ensuring accurate predictions for both work-related and leisure trips.


## Dataset

The dataset used in this project is sourced from travel booking data provided by Mr. Bilit website. The dataset includes information from various users and their travel bookings, including trip details, personal information, and ticket attributes.

**Note:** The dataset is proprietary, and thus, its publication is not permitted.

### Dataset Description

The dataset consists of travel booking records and includes the following columns:

| Column                  | Description                                        |
|-------------------------|----------------------------------------------------|
| `Created`               | Timestamp when the booking was made               |
| `CancelTime`            | Timestamp when the ticket was canceled            |
| `DepartureTime`         | Scheduled departure time of the trip              |
| `BillID`                | Purchase ID                                       |
| `TicketID`              | Ticket ID                                         |
| `ReserveStatus`         | Customer payment status                           |
| `UserID`                | Unique user ID                                    |
| `Male`                  | Gender of the passenger                           |
| `Price`                 | Price of the ticket without discounts             |
| `CouponDiscount`        | Discount applied to the ticket                    |
| `From`                  | Departure location                                |
| `To`                    | Destination location                              |
| `Domestic`              | Whether the trip is domestic or international     |
| `VehicleType`           | Type of vehicle used for the trip                 |
| `VehicleClass`          | Whether the vehicle is first-class or not         |
| `Vehicle`               | Specific vehicle used                             |
| `HashPassportNumber_p`  | Hashed passport number                            |
| `HashEmail`             | Hashed email address                              |
| `BuyerMobile`           | Hashed mobile number                              |
| `NationalCode`          | Hashed national ID                                |
| `Cancel`                | Whether the ticket was canceled                   |
| `TripReason`            | Reason for the trip (target variable)             |


### Dataset Location

- **Data/**: This folder will contain the dataset files.
- **Notebook/**: This folder will house your Jupyter notebooks. **Currently, we are working within the Notebook directory.**

## Project Structure

The main folders and files in the project are structured as follows:

```plaintext
Travel-Purpose-Prediction/
├── Data/
│   └── [dataset files will be here]
├── Notebook/
│   └── [your Jupyter notebooks will be here]
└── README.md
```

## Feature Engineering and Data Preprocessing

- **Identifying and creating new features** 
- **Handling missing values** 
- **Encoding categorical variables** 
- **Scaling numerical features** 
- **Splitting the dataset**

## Model Training

We used the **XGBoost** algorithm for classification to predict whether a booking is for work or leisure based on the extracted features.

## Model Performance

The model achieved the following F1 scores:
- **Training Set:** 0.7949
- **Test Set:** 0.6974

## Requirements
To run this project, you'll need the following Python libraries:
- `pandas`
- `scikit-learn`
- `xgboost`
