Hospital Claim Process Navigation Agent 

An interactive hospital insurance claim assistant built with LangGraph, LangChain, and Google Gemini 1.5 Flash, designed to guide patients through either Cashless or Reimbursement claim processes in a structured, conversational flow.

    📌 Features

-Step-by-step claim navigation for both claim types:

>Cashless Claim → pre-authorization, discharge approvals, and post-hospital benefits

>Reimbursement Claim → document collection, claim form guidance, and submission advice

-Natural Language Classification of patient queries into predefined process nodes

-Custom replies mapped to claim stage

-Debug-friendly logging for node classification

-Secure API Key handling (no hardcoded keys)

-Extendable LangGraph flow for adding more hospital processes

    🛠 Installation

-Clone this repository

>git clone https://github.com/MATHEW241197/AI_Agent/claim-process-navigator-agent-langgraph.git

>cd claim-process-navigator

-Install dependencies

>pip install -qU google-generativeai==0.8.5 google-ai-generativelanguage==0.6.15 \

>langgraph langchain langchain-google-genai openai

    🔑 API Key Setup

-This project uses Google Gemini API.

-Get your API key from Google AI Studio.

-You will be prompted to enter the key securely when running the script:

>import getpass, os

>os.environ['GOOGLE_API_KEY'] = getpass.getpass("Enter Gemini API Key: ")

    ▶️ Usage

-Run the script:

>python claim_navigator.py

Flow:

1.Select claim type → "Cashless" or "Reimbursement"

2.Describe your query → e.g., “I need to check my pre-auth approval.”

3.Agent classifies and responds with the next step in your claim process.

    📂 Project Structure

claim-process-navigator

    │
    ├── Main
      ├── Claim_Process_Navigator_Agent.ipynb                 # Main notebook
      ├── PYTHON_CODE.txt                                     # Python code 
    ├── samples
      ├── My_langgraph-Medical_Assistant_Agent.ipynb          # Sample project with different idea
    ├── docs
      ├── image.png                                           # UI image
      ├── Report.pdf                                          # Project report 
    ├── README.md                                             # Project documentation
    └── requirements.txt                                      # Python dependencies 

Flowchart given above is the file directory

     🔄 How It Works

1.LangGraph State Machine

-Nodes represent specific claim steps.

-Edges define conversational flow.

2.Gemini Model Classification

-Uses ChatGoogleGenerativeAI to map patient query → process node.

3.Predefined Response Map

-Returns exact, policy-compliant answers per claim stage.

    🗺 Claim Process Flow Diagram

Flowchart top to down

    A[Start: Select Claim Type] --> B{Claim Type?}
    B -->|Cashless| C[Cashless Claim Flow]
    B -->|Reimbursement| D[Reimbursement Claim Flow]

    C --> C1[Confirm Network]
    C1 --> C2[Pre-auth Request]
    C2 --> C3[Pre-auth Query]
    C3 --> C4[Pre-auth Approved]
    C4 --> C5[Discharge Request]
    C5 --> C6[Discharge Query]
    C6 --> C7[Discharge Approved]
    C7 --> C8[Post-hospital Claims]
    C8 --> Z[End]

    D --> D1[Document Collection]
    D1 --> D2[Claim Form Guidance]
    D2 --> D3[Hospital Part Completion]
    D3 --> D4[Submission Advice]
    D4 --> D5[Claim Process Complete]
    D5 --> Z[End]

This is the entire workflow of the agent.

    📜 Example Interaction

Welcome to ADAM Hospital. Are you here for 'Cashless' or 'Reimbursement' claim?

Cashless

Please describe your concern:

I want to know how long pre-authorization takes.

[DEBUG] Node classified as: cashless_preauth_request

Once submitted, your pre-authorization request is sent to the insurer/TPA which is typically completed within about 1 hour of submission.

    📌 Future Enhancements

-Multi-lingual support

-Integration with hospital CRM systems

-Web-based chatbot interface

-Additional claim categories

    📄 License

This project is licensed under the MIT License.

    🤝 Contributing

Contributions are welcome!

-Fork the repo

-Create a new branch (feature-new-idea)

-Commit changes

-Submit a pull request

    👨‍💻 Author

Mathew Abraham

🔗 www.linkedin.com/in/drmathewabraham | https://github.com/MATHEW241197
