LinkedIn Post Generator (AI Reflex Agent)


    📌 Overview

The LinkedIn Post Generator (AI Reflex Agent) is an interactive Jupyter Notebook tool that uses Google Gemini AI to create high-quality, personalized LinkedIn posts in seconds. With a simple form interface powered by ipywidgets, you can customize post tone, type, audience, key points, and even hashtags—without writing a single line of prompt each time.

This project is perfect for:

-Professionals looking to write impactful career updates.

-Students wanting to share achievements or tips.

-Recruiters posting hiring updates.

-Thought leaders sharing industry insights.


    🚀 Features

-Customizable Inputs: Topic, audience, tone, content type, key points, goals, CTAs, hashtags, mentions, and links.

-Multiple Tones: Professional, casual, witty, motivational, informative, reflective, inspirational, and conversational.

-Post Types: Career updates, storytelling, hiring posts, tips/advice, project progress, resource sharing, and more.

-Additional Options:
>Add emojis

>Use line breaks for readability

>Include personal reflections

>Length Control: Limit the post to a specific character count.

-AI-Powered: Uses Google Gemini 2.5 Flash for fast, high-quality generation.


    🛠️ Installation & Setup

1️⃣ Clone the repository

>git clone https://github.com/<your-username>/linkedin-post-generator.git

>cd linkedin-post-generator

2️⃣ Install dependencies

>Open the .ipynb file in Google Colab or Jupyter Notebook and run:

>!pip install google-generativeai --quiet

>!pip install ipywidgets --quiet

>jupyter nbextension enable --py widgetsnbextension


    🔑 API Key Setup

This project uses Google Gemini API.

Get your API key from: Google AI Studio

When prompted in the notebook:

Enter the Gemini API Key: *****


📋 How to Use

-Open the .ipynb file in Google Colab or Jupyter Notebook.

-Run all cells until you see the LinkedIn Post Generator form.\

-Fill in:

>Post Topic – e.g., "Promoted to Senior Analyst at XYZ!"

>Audience – e.g., "Students, HRs, Working Professionals"

>Tone – e.g., "Professional"

>Type – e.g., "Career Updates"

>Key Point – e.g., "Gratitude for mentors and peers"

>Goal – e.g., "Inspire"

>Call to Action (CTA) – e.g., "Share your journey!"

>Hashtags – e.g., "#Leadership #Career"

>Optional: Mentions, links, emoji toggle, line breaks, reflection.

-Click Generate Post.

-Copy and paste your AI-crafted post to LinkedIn.


    📂 Project Structure

linkedin-post-generator

    │
    ├── Main
      ├── LinkedIn_Post_Generator.ipynb   # Main notebook
      ├── PYTHON_CODE.txt                 # Python code 
    ├── docs
      ├── image.png                       # UI image
      ├── Report.pdf                      # Project report
    ├── samples                           # Sample project with different idea
    ├── README.md                         # Project documentation
    └── requirements.txt                  # Python dependencies 

Flowchart given above is the file directory

    ⚡ Example Output

Post Topic: Promoted to Senior Analyst at XYZ

Tone: Professional

Type: Career Updates

Goal: Inspire

CTA: Share your thoughts!

Hashtags: #CareerGrowth #Promotion

Generated Post:

Thrilled to share that I’ve been promoted to Senior Analyst at XYZ!
This milestone wouldn’t have been possible without the guidance of my mentors, support of my peers, and the trust of my leadership team.To all professionals striving for growth—keep learning, stay curious, and embrace challenges as opportunities.🚀
Share your thoughts on your biggest career breakthrough!
#CareerGrowth #Promotion #LinkedIn #SuccessStories


    🧠 How It Works

ipywidgets creates a dynamic form for input.

Your inputs are compiled into a detailed prompt for Gemini AI.

Google Gemini API generates a LinkedIn-ready post.

Output is displayed in Markdown format for easy copying.


    📜 License

This project is licensed under the MIT License – feel free to use, modify, and share.


    🤝 Contributing

Contributions are welcome!

-Fork the repo

-Create a new branch (feature-new-idea)

-Commit changes

-Submit a pull request


    💡 Future Improvements

-Add support for multiple social platforms (Twitter, Instagram captions).

-Integrate direct posting to LinkedIn API.

-Save generated posts history.


    👨‍💻 Author

Mathew Abraham

🔗 www.linkedin.com/in/drmathewabraham | https://github.com/MATHEW241197

