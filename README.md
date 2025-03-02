SIEM Anomaly Detection with GUI
This project demonstrates a simple Security Information and Event Management (SIEM) anomaly detection system using machine learning, with a graphical user interface (GUI) for uploading and visualizing data. The GUI is built with ipywidgets and runs directly within a Jupyter Notebook.

Project Overview
In this project, the goal is to:

Upload log data: Allows the user to upload log data from a CSV file.
Process and analyze the data: Uses machine learning algorithms (e.g., Isolation Forest) to detect anomalies in the log data.
Visualize results: The user can visualize data trends such as network traffic or bytes sent over time using interactive plots.
Features
Log Data Upload: Users can upload CSV files containing log data.
Anomaly Detection: The model uses an Isolation Forest algorithm to detect outliers (anomalies) in the log data.
Data Visualization: Once the data is uploaded and processed, users can visualize the trends in the log data, such as the bytes sent over time.
Installation
Prerequisites
You will need to have the following Python libraries installed:

pandas
numpy
matplotlib
seaborn
ipywidgets
scikit-learn
To install the necessary libraries, you can run:

bash
Copy code
pip install pandas numpy matplotlib seaborn ipywidgets scikit-learn
Running the Project in Jupyter Notebook
Clone the repository to your local machine:

bash
Copy code
git clone https://github.com/your-username/siem-anomaly-detection.git
cd siem-anomaly-detection
Open the Jupyter Notebook:

bash
Copy code
jupyter notebook
Run the notebook cells in sequence:

The first section loads the necessary libraries.
The second section allows users to upload the log data.
The third section analyzes the data using machine learning.
The final section visualizes the data trends and anomalies.
Project Structure
bash
Copy code
siem-anomaly-detection/
│
├── README.md                  # Project overview
├── anomaly_detection.ipynb     # Jupyter Notebook with the code
├── requirements.txt            # List of required Python libraries
How to Use the GUI
Upload Log Data:

Click the "Choose File" button to upload a CSV file containing log data (e.g., timestamp, bytes_sent, etc.).
Click the "Upload CSV" button to load the data into the notebook.
Plot Data:

Once the data is successfully uploaded, click the "Plot Data" button to visualize trends such as bytes_sent over time.
Anomaly Detection:

The uploaded data will automatically be processed to detect anomalies using the Isolation Forest model. Anomalies will be identified based on specific features in the dataset.
Example Dataset Structure
An example CSV file may have the following structure:

timestamp	event_id	source_ip	destination_ip	bytes_sent	bytes_received
2024-12-22 12:00:00	1001	192.168.1.1	192.168.1.10	500	1500
2024-12-22 12:01:00	1002	192.168.1.1	192.168.1.11	300	1800
...	...	...	...	...	...
Columns:
timestamp: The date and time of the log event.
event_id: An identifier for the event.
source_ip: The source IP address of the request.
destination_ip: The destination IP address of the request.
bytes_sent: The number of bytes sent.
bytes_received: The number of bytes received.
Contributing
If you have suggestions or improvements, feel free to fork the repository, make changes, and create a pull request. Contributions are welcome!

License
This project is licensed under the MIT License - see the LICENSE file for details.