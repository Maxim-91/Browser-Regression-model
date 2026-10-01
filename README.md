# Browser Regression Model

A simple browser-based application for using a **linear regression model** directly in HTML and JavaScript.

The application does not use external libraries for the regression calculations. The user can load a CSV file, select a target variable and one or more input variables, choose the train/test split, and run the regression model directly in the browser.

## How It Works

1. Click **"Vie tiedot CSV-muotoon"** and select a CSV file from the computer.
2. The CSV data is displayed in a table below.
3. The application detects the numerical columns from the CSV file.
4. The user selects one numerical column as the **target**.
5. The other numerical columns can be selected or unselected as input variables.
6. At least one input variable must be selected to run the regression.
7. The user can change the **Train/Test split** using the input fields or the slider.
8. The default split is **70% training data and 30% test data**.
9. The application calculates the linear regression model using the selected data.
10. The following results are displayed:
    * R² score
    * Mean Absolute Error (MAE)
    * Mean Squared Error (MSE)
    * Root Mean Squared Error (RMSE)
11. The calculated regression formula is also displayed.
12. A scatter plot of **y_test and y_pred** is shown below the results.

The regression calculations are implemented directly in JavaScript without using machine learning or regression libraries.

## Test Data

Two CSV files are included in the repository for testing the regression model.

### Data01.csv

`Data01.csv` contains real GPS data collected using the **Sensor Logger** application on an Android device.

The data was collected using **four different methods** on the same route during two days.

### Data02.csv

`Data02.csv` contains computer activity data collected using the Python data collection program:

[GitHub link: Task-Manager-Data-Collector](https://github.com/Maxim-91/Task-Manager-Data-Collector.git)

The computer performance data was collected for approximately **5–7 minutes** while different programs were used to create different levels of computer load.

The collected data includes computer performance measurements such as running processes, CPU usage, RAM usage  and disk activity.

## Video Demonstration

[YouTube](https://youtu.be/YtJEMQAIZMU)

## AI Tool Usage

The `index.html` code was generated with the help of **ChatGPT**. The design was slightly improved manually and the application was tested with different datasets.

**Gemini** was also used to review and check the generated code.
