🏥 Hospital Waste Management AI Multi-Agent System


📌 Overview

The Hospital Waste Management AI Agent System is an automated, multi-agent workflow that uses AI to validate, route, and log biomedical waste data in real-time.
Built on the Relay App and powered by Google Forms, Excel, Email Automation, and GPT-5, this system ensures SDG 12: Responsible Consumption and Production compliance while reducing manual errors, improving efficiency, and enhancing hospital safety.

This project is perfect for:

-Hospitals aiming for zero biomedical waste segregation errors

-Sustainability officers seeking SDG 12 compliance

-Healthcare administrators wanting audit-ready logs

-Teams looking to reduce environmental impact of waste


🚀 Features

-Real-Time Validation – Checks waste category vs. description instantly

-Smart Routing – Directs waste for internal handling or external vendor pickup

-Error Logging – Records segregation mistakes and notifies the responsible staff

-Automated Notifications – Emails sent to relevant disposal teams

-SDG 12 Aligned – Promotes recycling, safe disposal, and reduced contamination


🛠 Installation & Setup

1️⃣ Clone the repository

>git clone https://github.com/<your-username>/hospital-waste-ai-agent.git 
>cd hospital-waste-ai-agent

2️⃣ Set up environment

-Create a Google Form matching required fields (email, date/time, department, category, description, weight, disposal method)

-Connect the form responses to a Relay App workflow

-Configure your GPT-5 API key in Relay

3️⃣ Link to Excel & Email System

-Ensure Excel log file is connected for error tracking

-Set up email triggers in Relay for notifications


📋 How to Use

-Staff fills out the Google Form for waste disposal

-Agent 1 validates category vs. description

>If mismatch → Agent 2 logs error & sends correction email

>If match + Internal → Agent 3 sends action steps to internal disposal authority

>If match + External → Agent 4 routes to Incineration or Recycling team and confirms collection


📂 Project Structure

hospital-waste-ai-agent

    │
    ├── Main
      ├── Hospital waste Management.pptx  # Project PPT
    ├── docs
      ├── image                           # UI image
      ├── Cover Note.pdf                  # Project report
      ├── Project Lean Canvas.pdf         # Project report
    ├── samples                           # Sample project with different idea
    ├── README.txt                        # Project documentation
    └── requirements.txt                  # Python dependencies 


⚡ Example Workflow

Input: "Yellow bin, infected cotton" → ✅ Match → Internal Disposal

Input: "Black bin, used gloves" → ❌ Mismatch → Error log + correction email


🧠 How It Works

-Google Forms – Data collection

-Relay App + GPT-5 – Validation & decision logic

-Excel – Centralized error logging

-Email Automation – Timely notifications to staff & vendors

📜 License

This project is licensed under the MIT License – free to use, modify, and distribute.

🤝 Contributing

-Fork the repo

-Create a branch (feature-new-improvement)

-Commit changes

-Submit a pull request


💡 Future Improvements

-QR code scanning for bins

-Live waste analytics dashboard

-Voice-based waste entry for field workers

👨‍💻 Author


Dr. Mathew Abraham

🔗 www.linkedin.com/in/drmathewabraham | https://github.com/MATHEW241197
