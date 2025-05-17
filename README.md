Alpha Vantage Demo
This repository demonstrates how to use the Alpha Vantage API for retrieving financial data. Follow the steps below to securely store your API key, set up a virtual environment, install dependencies, and run the program.

1. Securely Storing the API Key
Before running the program, you need to store your Alpha Vantage API key securely.

Using a .env File (Recommended)
Create a .env file in the root directory of the project.

Add the following line, replacing your_api_key_here with your actual API key:

ALPHA_VANTAGE_API_KEY=your_api_key_here
The program will read this key using the dotenv package.

Alternative: Using Environment Variables
If you prefer, you can set the API key directly in your system environment variables:

Windows (Command Prompt):
set ALPHA_VANTAGE_API_KEY=your_api_key_here
macOS/Linux (Terminal):
export ALPHA_VANTAGE_API_KEY=your_api_key_here
2. Setting Up a Virtual Environment
It is recommended to use a virtual environment to manage dependencies.

Create a Virtual Environment
Windows (Command Prompt / PowerShell):
python -m venv venv
macOS/Linux (Terminal):
python3 -m venv venv
Activate the Virtual Environment
Windows (Command Prompt):
venv\Scripts\activate
Windows (PowerShell):
venv\Scripts\Activate.ps1
macOS/Linux (Terminal):
source venv/bin/activate
3. Installing Dependencies
Once the virtual environment is activated, install the required packages using requirements.txt:

pip install -r requirements.txt
This will install all necessary libraries such as requests, pandas, python-dotenv, and others.

4. Running the Program
Ensure the virtual environment is activated.

Run the Python script:

python main.py
or if using Python 3 explicitly:

python3 main.py
The script will fetch financial data using your stored API key.

5. Deactivating the Virtual Environment
Once you're done, you can deactivate the virtual environment:

deactivate
6. Additional Notes
If you encounter any errors related to missing dependencies, try running:
pip install --upgrade pip
pip install -r requirements.txt
To prevent exposing your API key, DO NOT commit your .env file to version control. Add .env to your .gitignore file:
.env
If you need a new API key, generate one from Alpha Vantage.
