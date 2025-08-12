Health Myth Buster Agent (RAG-based)

This project is an interactive Retrieval-Augmented Generation (RAG) agent designed to debunk health myths using trusted online sources.It scrapes specified websites, stores their content in a vector database, and uses Google Gemini AI to generate fact-based answers.

    🚀 Features

-Web scraping from trusted health sites with depth and page limits.

-Text cleaning & chunking for optimal embedding.

-FAISS vector search for fast and relevant retrieval.

-Google Gemini AI integration for generating clear, evidence-based answers.

-Jupyter Notebook widgets UI for easy interaction.

-Fully customizable:

>Choose websites to scrape.

>Set scraping depth & page limits.

>Ask any health-related question.

    🛠️ Tech Stack

-Python

-BeautifulSoup4 – HTML parsing & scraping

-FAISS – Vector similarity search

-SentenceTransformers – Text embeddings

-Google Gemini API – Answer generation

-ipywidgets – Interactive UI in Jupyter Notebook

    📦 Installation

>!pip install requests beautifulsoup4 numpy faiss-cpu sentence-transformers google-generativeai ipywidgets

    📋 How It Works

1.Scraping

The tool starts by scraping the specified health websites up to a given depth and page limit.

2.Processing

Text is cleaned, chunked, and converted into vector embeddings using all-MiniLM-L6-v2.

3.Indexing

FAISS stores these embeddings for quick semantic search.

4.Retrieval

Relevant chunks are retrieved based on your query.

5.Generation

Gemini AI uses these chunks to answer, citing the retrieved content.

    ▶️ Usage

1.Run the notebook in Jupyter or Google Colab.

2.Enter your Gemini API key when prompted.

3.Input one or more trusted health website URLs (one per line).

4.Set:

-Depth: How many link levels to follow.

-Max Pages: Limit of total pages scraped.

5.Click Scrape & Build Index.

6.Enter a health claim and click Myth Buster Answer.

7.View the AI-generated evidence-based answer.

    📌 Example

Input Claim:

Does garlic cure heart attacks?

AI Answer:

✅ Based on WHO and Mayo Clinic sources, garlic does not cure heart attacks.
It may help maintain heart health when part of a balanced diet, but it is not a treatment for acute cardiac events.

    ⚠️ Disclaimer

This tool is for educational purposes only. It does not provide medical advice. Always consult a qualified healthcare professional for medical concerns.

    📄 License

This project is licensed under the MIT License – feel free to modify and share.

    🤝 Contributing

Contributions are welcome!

-Fork the repo

-Create a new branch (feature-new-idea)

-Commit changes

-Submit a pull request

    🔮 Future Improvements

-Add credibility scoring for sources.

-Automated scraping processes.

-Deploy as a web app for wider access.

    👨‍💻 Author

Mathew Abraham

🔗 www.linkedin.com/in/drmathewabraham | https://github.com/MATHEW241197
