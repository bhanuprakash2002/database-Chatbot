# Database ChatBot 🤖

The **Database ChatBot** is a Streamlit-based application designed to allow users to query a **MySQL** or **PostgreSQL** database using natural language. By leveraging **Langchain** for natural language processing, it automatically generates SQL queries based on user input. The chatbot also supports multilingual responses, provides text-to-speech functionality, and allows users to download responses or copy them to the clipboard.

## 🚀 Features

- **Natural Language Querying**: Generate SQL queries automatically based on user questions in plain text.
- **Database Connectivity**: Seamlessly connect to **MySQL** or **PostgreSQL** databases.
- **Multilingual Support**: Responds in multiple languages.
- **Text-to-Speech**: Convert text responses into speech and download them as MP3 files.
- **Download & Clipboard Features**: Download text responses, audio responses, and copy text responses to the clipboard.
- **Session Management**: Chat history persists during the session, and you can clear it at any time.

## 📷 Chatbot Interface
**User Input & Customization**

![1](https://github.com/user-attachments/assets/430a3ad2-4e1f-4dc9-8fef-30a6e948babc)

**Database Connection**

![2](https://github.com/user-attachments/assets/634f74d5-e117-4336-848c-c8f8eb97a2f9)

**Generated Response**

![3](https://github.com/user-attachments/assets/c3a1d8e9-feab-4a02-86e7-44b5767f5a68)

## 📦 Installation

1. **Clone the Repository**:

   ```bash
   git clone https://github.com/CodeWizardl/Database-Chatbot.git
   cd Database-Chatbot
   ```

2. **Install Dependencies**:

   ```bash
   pip install -r requirements.txt
   ```

3. Download and install the LLaMA 3 model from [Ollama](https://ollama.com/):

   - Go to [Ollama](https://ollama.com/) and download the LLaMA 3 model.
   - Follow the installation instructions provided on the Ollama website.
   - Once installed, ensure that it is properly configured and accessible from your environment.

4. **Run the Streamlit Application**:

   ```bash
   streamlit run app.py
   ```

## ⚙️ Usage

1. **Connect to the Database**: 
   - In the sidebar, select **MySQL** or **PostgreSQL** and provide connection details (host, port, username, password, and database name).
   
2. **Ask Questions**:
   - Type a question in natural language (e.g., *How many employees are in the database?*).
   
3. **View SQL Query and Response**:
   - The chatbot will generate the SQL query (e.g., `SELECT COUNT(*) FROM employees;`) and display the result as a natural language response.

4. **Multilingual Support**:
   - Choose a language for responses from the sidebar (English, Hindi, Spanish, etc.).
   
5. **Actions**:
   - **Download**: Download the response as text or audio.
   - **Copy to Clipboard**: Copy the text response to the clipboard.
   - **Text-to-Speech**: Listen to the response or download it as an MP3 file.

## 🛠 Example Flow

1. **User question**: *How many products are available?*
2. **Generated SQL query**: `SELECT COUNT(*) FROM products;`
3. **Response**: *There are 100 products available.*
4. **Available actions**:
   - Download the response as text or audio.
   - Copy the text to the clipboard.
   - Listen to the audio directly in the app.

## 🧩 Supported Languages

The chatbot currently supports the following languages:

- **Indian Languages**: Hindi, Bengali, Telugu, Tamil, Gujarati, Kannada, Punjabi, Malayalam
- **Foreign Languages**: English, Spanish, French, German, Italian, Portuguese, Arabic, Russian

## 🎤 Text-to-Speech (TTS)

Using **gTTS** (Google Text-to-Speech), users can convert text responses into audio files, which are available for download. This feature is especially useful for multilingual responses.

## ✏️ Customization

- **Query Generation**: The application uses **Langchain** to generate SQL queries based on natural language input.
- **Text-to-Speech**: The app leverages the **gTTS** library for generating speech from text, supporting the same set of languages.
- **Translation**: For translating responses, the **Translate** library is used, ensuring accurate translations into the supported languages.

## 💾 Requirements

- **Python** (3.8+)
- **Streamlit**
- **Langchain Community** (for query generation)
- **gTTS** (for text-to-speech)
- **Pyperclip** (for clipboard operations)
- **Translate** (for translations)

## 🔮 Future Work

We plan to enhance the **Database ChatBot** with the following features:

1. **Support for More Databases**:
   - Extend connectivity to other popular databases like **MongoDB**, **SQLite**, and **Oracle**.

2. **Advanced Query Optimization**:
   - Implement advanced query optimization techniques to handle more complex queries and improve response times for large datasets.

3. **Contextual Conversations**:
   - Introduce session-based contextual awareness so the chatbot can maintain context and follow up on previous queries, improving conversational flow.

4. **Voice Input Support**:
   - Integrate voice input features, allowing users to interact with the chatbot using speech, with real-time transcription into text queries.

5. **Improved Multimodal Support**:
   - Extend support for image-based queries where users can upload charts, graphs, or other images, and the chatbot will analyze and respond based on the visual data.

## 📄 License

This project is licensed under the MIT License.
