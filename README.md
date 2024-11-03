# Multi-Topic RAG Chatbot

A conversational AI system that uses Retrieval-Augmented Generation (RAG) to provide informed responses across multiple topics. The chatbot leverages LangChain, ChromaDB, and OpenAI to process and retrieve information from a curated collection of documents.

Chatbot link: https://875627278d9993e811.gradio.live
## Features

- Multi-topic support covering:
  - Python Programming
  - Machine Learning
  - UAE Information
- RAG-enhanced responses using document retrieval
- Conversation memory to maintain context
- User-friendly Gradio interface
- Support for both PDF and text file sources

## Prerequisites

- Python 3.8+
- Jupyter Notebook
- OpenAI API key
- LangChain API key (optional, for tracing)

## Installation

1. Clone the repository:
```bash
git clone https://github.com/abdelrahmanomar1/Multi-Topic-RAG-Chatbot.git
cd Multi-Topic-RAG-Chatbot
```

2. Create and activate a virtual environment:
```bash
# For macOS/Linux
python3 -m venv myenv
source myenv/bin/activate

# For Windows
python -m venv myenv
myenv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
pip install jupyter  # Make sure Jupyter is installed
```

4. Create a `.env` file with your API keys:
```env
OPENAI_API_KEY=your_openai_api_key
LANGCHAIN_API_KEY=your_langchain_api_key
LANGCHAIN_TRACING_V2=true
```

## Project Structure
```
.
├── Data/
│   ├── Python/
│   │   ├── The 23 Top Python Interview Questions & Answers For 2024 | DataCamp.pdf
│   │   └── Cheat-Sheet.txt
│   ├── AI_ML/
│   │   ├── Machine Learning Cheatsheet.pdf
│   │   └── Top 30 AI Interview Questions & Answers For 2024 | DataCamp.pdf
│   └── UAE/
│       ├── uae_info.txt
├── chatbot.ipynb
├── requirements.txt
├── .env
└── README.md
```

## Usage

1. Place your reference documents in the appropriate folders under the `Data` directory.

2. Start Jupyter Notebook:
```bash
jupyter notebook
```

3. Open `chatbot.ipynb` in the Jupyter interface

4. Run all cells in the notebook (Cell → Run All)

5. Access the Gradio interface in your web browser (default: http://127.0.0.1:7860)

6. Select a topic from the dropdown menu and start chatting!

## Features in Detail

### Document Processing
- Supports both PDF and text files
- Automatically splits documents into manageable chunks
- Creates efficient vector embeddings for retrieval using ChromaDB

### Conversation Management
- Maintains context across multiple exchanges
- Provides relevant information from the document base
- Supports natural conversation flow

### User Interface
- Clean, intuitive Gradio interface
- Easy topic selection
- Real-time responses

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/YourFeature`)
3. Commit your changes (`git commit -m 'Add some feature'`)
4. Push to the branch (`git push origin feature/YourFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License.

## Author

AbdelrahmanRasheed AL-Omari
- GitHub: [@AbdelrahmanRasheedAlOmari](https://github.com/AbdelrahmanRasheedAlOmari)

## Acknowledgments

- OpenAI for the GPT model
- LangChain for the RAG framework
- Gradio for the user interface
- ChromaDB for vector storage
