# 🐳 Dockerfile Generator

A GenAI powered tool that generates optimized Dockerfiles based on programming language input. This project uses Ollama with the Llama3 model to create Dockerfiles following best practices.

## 📋 Prerequisites

### Installing Ollama

1. **Download and Install Ollama**
   ```bash
   # For Linux
   curl -fsSL https://ollama.com/install.sh | sh

   # For MacOS
   brew install ollama
   ```

2. **Start Ollama Service**
   ```bash
   ollama serve
   ```

3. **Pull Llama3 Model**
   ```bash
   ollama pull llama3.1:8b
   ```

## 🚀 Project Setup

1. **Create Virtual Environment**
   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Linux/MacOS
   # or
   .\venv\Scripts\activate  # On Windows
   ```

2. **Install Dependencies**
   ```bash
   pip3 install -r requirements.txt
   ```

3. **Run the Application**
   ```bash
   python3 generate_dockerfile.py

##for Hosted##
I used Google AI Studio to generate API keys and mentioned that key in the generate_dockerfile_gemini.py file

-> Run " pip3 install google.generativeai "

and then run " python3 generate_dockerfile_gemini.py "

## 💡 How It Works

1. The script takes a programming language as input (e.g., Python, Node.js, Java)
2. Connects to the Ollama API running locally
3. Generates an optimized Dockerfile with best practices for the specified language
4. Returns the Dockerfile content with explanatory comments

## 📝 Example Usage

```bash
python3 generate_dockerfile.py
Enter programming language: python
# Generated Dockerfile will be displayed...
```

## 🏆 Troubleshooting
- Make sure Ollama service is running before executing the script.
- Ensure the correct model is downloaded.
- Adapt best practices for other programming languages as needed.
