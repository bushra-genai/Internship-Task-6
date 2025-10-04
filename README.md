# Internship-Task-6

📈 Market Research Agent 2 — Streamlit App

An intelligent Market Research Agent that automates competitor analysis and market scanning.
It integrates Tavily Search API for real-time web research and Groq LLM (via LangChain) for professional synthesis of market insights.

Built with Streamlit for an interactive dashboard experience.

🚀 Features

🔎 Live Web Search using Tavily API

🤖 LLM-powered Report Generation with Groq (LLaMA 3.1 models)

🏷️ Automatic competitor extraction from search results

💲 Price parsing in PKR from product listings & snippets

📝 Generates a comprehensive market report:

Competitors & their specs

Current prices in PKR (approximate)

Key features summary

Customer sentiment overview

Final recommendations

📂 Export options: Download reports as TXT or JSON

🖥️ Clean Streamlit UI with expandable logs & raw sources

📋 Requirements

Python 3.9+ is recommended.

Install dependencies via:

pip install -r requirements.txt

requirements.txt (sample)
streamlit>=1.20.0
requests>=2.28.0
python-dotenv>=1.0.0
langchain-groq>=0.1.0    # for ChatGroq client
tavily>=0.1.0            # Tavily search client
numpy>=1.23.0


(adjust versions based on your environment)

🔑 API Keys

This app needs two API keys:

Tavily API Key 

Groq API Key
Paste your keys into the sidebar inputs when running the app.
⚠️ Keys are stored only in session memory and not saved to disk.

▶️ Usage

Run the app locally:

streamlit run app.py

Steps:

Launch the app.

Enter API keys in the sidebar.

Type a product name / research objective (e.g., Nexus Smartwatch Pro 2).

Click Start Research.

Wait for 20–60 seconds while the agent gathers data.

View the final market analysis report + raw data logs.

Optionally, download reports in TXT or JSON.

📂 Project Structure
├── app.py              # Main Streamlit app
├── requirements.txt    # Python dependencies
├── README.md           # Project documentation

🛠️ How it Works

Initial Search → Finds top competitors/products from Tavily results.

Competitor Queries → For each, runs searches for:

Specs

Prices

Customer Reviews

Price Parsing → Extracts PKR values using regex.

LLM Summarization → Groq LLaMA model generates structured market insights.

Streamlit UI → Displays final report, raw logs, and export options.

✨ Example Output

Competitors Found: Apple Watch Series 9, Samsung Galaxy Watch 6, Huawei Watch GT 4

Final Report:

Apple Watch Series 9

Features: Always-on display, ECG, SpO2, fitness tracking

Price: PKR 145,000 (approx)

Sentiment: Customers praise build quality, but battery life still criticized.

Submit a PR

📜 License

This project is open-source under the MIT License.

👩‍💻 Author

Developed by Bushra ✨
