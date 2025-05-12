AI Home Search For Indonesia Region Especially Jabodetabek Malang & Surabaya
Desktop application that allows users to search for house properties based on keywords. This system is built using PyQt5 as the user interface and Flask as the backend server that manages data searches from two sources: Excel and CSV files containing house data in the Jabodetabek area.

📂 Features
🔍 Search for house properties based on keywords (house name or ad title).
📄 Displays search results from two data sources:
HOUSE DATA.xlsx
*jabodetabek_house_price.csv*
⚡ Interactive desktop interface based on PyQt5.
🔌 Communication between the frontend and backend uses HTTP (REST API).
🛠️ Project Structure
real-estate-search/
│
├── real_estate_app.py
├── ai_backend.py
├── DATA RUMAH.xlsx
├── jabodetabek_house_price.csv
└── README.md
▶️ How to Run
1. Install Required Libraries
"pip install pandas flask pyqt5 openpyxl"
2. Run Flask Backend
"python ai_backend.py"
3. Run Desktop Application
"python real_estate_app.py"
💡 How it Works
User types keywords in the desktop application. The application sends a POST request to the Flask server (localhost:5000/search) with JSON { "query": "keywords" }.
The backend looks for results from:
The HOUSE NAME column in Excel
The title column in CSV
The backend returns the results as JSON.
The GUI displays the search results on the screen.
