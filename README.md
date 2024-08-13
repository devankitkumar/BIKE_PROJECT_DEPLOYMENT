𝐔𝐬𝐞𝐝 𝐁𝐢𝐤𝐞 𝐏𝐫𝐢𝐜𝐞 𝐏𝐫𝐞𝐝𝐢𝐜𝐭𝐢𝐨𝐧

This project aims to predict the price of used bikes based on various factors such as brand, kilometers driven, ownership, age, and power. The prediction is made using a linear regression model trained on a dataset of used bikes.

𝐏𝐫𝐨𝐣𝐞𝐜𝐭 𝐒𝐭𝐫𝐮𝐜𝐭𝐮𝐫𝐞
    1. 𝐃𝐚𝐭𝐚𝐛𝐚𝐬𝐞 𝐂𝐫𝐞𝐚𝐭𝐢𝐨𝐧:: The database bikedata_db is created using SQLite, containing a table CarDetails that holds the relevant features.

   2.𝐃𝐚𝐭𝐚 𝐏𝐫𝐞𝐩𝐫𝐨𝐜𝐞𝐬𝐬𝐢𝐧𝐠: The data is cleaned by removing duplicates and handling missing values.
    Features like brand and owner are encoded into numerical values for model compatibility.

   3.𝐌𝐨𝐝𝐞𝐥 𝐓𝐫𝐚𝐢𝐧𝐢𝐧𝐠: A linear regression model is trained on the cleaned dataset to predict bike prices.
    The model achieves a training accuracy of approximately 73.4% and a test accuracy of 76.6%.

   4.𝐅𝐥𝐚𝐬𝐤 𝐖𝐞𝐛 𝐀𝐩𝐩𝐥𝐢𝐜𝐚𝐭𝐢𝐨𝐧:The application uses Flask to create a simple web interface for users to input bike details and get a price prediction.
    The model is loaded and predictions are made based on user inputs, which are passed through the Flask app.


𝐊𝐞𝐲 𝐅𝐮𝐧𝐜𝐭𝐢𝐨𝐧𝐬:
  Database Setup:

SQL queries are used to create the CarDetails table within bikedata_db.
Model Training:

Linear regression from the scikit-learn library is used for training the model, and the model is saved using joblib.
Web Interface:

The Flask application serves the HTML templates and handles prediction requests.
The /predict route processes user input, predicts the price, and displays it on the home page.


𝐑𝐮𝐧𝐧𝐢𝐧𝐠 𝐭𝐡𝐞 𝐏𝐫𝐨𝐣𝐞𝐜𝐭:
Setting Up:

Ensure all dependencies are installed. This includes Flask, pandas, numpy, scikit-learn, and joblib.
Running the App:

Start the Flask server by running the app.py file.
Navigate to http://127.0.0.1:5000/ in your web browser to interact with the prediction interface.


𝐒𝐮𝐦𝐦𝐚𝐫𝐲
This project combines data preprocessing, machine learning, and web development to create a complete application capable of predicting the prices of used bikes based on user inputs.

