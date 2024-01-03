
This application allows you to load a PDF and ask questions about it using natural language. The application uses a OpenAi's LLM to generate a response about your PDF. The LLM will not answer questions unrelated to the document.

## Working

The application works by splitting the PDF into smaller chunks so that they can be fed into the LLM. It uses OpenAI embeddings to create vector representations of the chunks. The application then finds the chunks that are semantically similar to the question that the user asked and feeds those chunks to the LLM to generate a response.

## Installation

Please clone the repository and install the requirements:

```
pip install -r requirements.txt
```

You will also need to add your OpenAI API key to the `.env` file.

## Usage

To use the application, run the `main.py` file with the streamlit CLI (after having installed streamlit): 

```
streamlit run app.py
```

