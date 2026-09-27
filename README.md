# ai-local-discovery-automation
AI-powered local discovery assistant built with n8n, APIs and AI.
AI-Powered Local Discovery & Recommendation Assistant

An AI-powered automation that helps users discover relevant places around a specific location.

The user provides a location, the type of place they are looking for, and a search radius. The workflow retrieves available location data through an external API, processes the results, and uses AI to organize, filter, rank, and summarize the most relevant options before delivering the results to the user.

🚀 What It Does

Instead of simply returning a large list of nearby places, the system attempts to turn raw location data into a more useful, personalized recommendation.

User provides

* 📍 Location / area
* 🏷️ Type of place
* 🌍 Country
* 📌 State / region
* 📏 Search radius
* 📧 Email address

The workflow

1. Receives the user’s request through an n8n form.
2. Processes the location and search parameters.
3. Queries a location/business data API.
4. Receives the available places.
5. Processes the returned data.
6. Uses AI to filter and rank results based on relevance.
7. Generates a short personalized summary.
8. Formats the results.
9. Sends the final recommendations to the user’s email.

🧠 Why AI?

A traditional location search can return many results without helping the user understand which ones are most relevant.

The AI layer adds an interpretation step.

Instead of:

Restaurant A
Restaurant B
Restaurant C
Restaurant D
Restaurant E

The system can organize the available information into something easier to understand, such as:

Based on the search criteria, these options appear most relevant. Option A is closest, while Option B has the strongest match based on the available information.

The AI is instructed to work only with information returned by the data source and avoid inventing unavailable details.

🛠️ Technologies

* n8n
* REST APIs
* AI / LLM integration
* Location & business data APIs
* Webhooks / Forms
* JSON
* Email automation

🔄 Workflow

User
  ↓
n8n Form
  ↓
Search Parameters
  ↓
Location / Business API
  ↓
Raw Results
  ↓
Data Processing
  ↓
AI Relevance & Summary
  ↓
Formatted Results
  ↓
Email



User Form

n8n Workflow

Example Results

🎯 Key Features

* Location-based search
* Custom search radius
* Multiple place categories
* API integration
* AI-powered result filtering
* AI-generated summaries
* Personalized recommendations
* Automated email delivery
* Structured JSON data processing

📚 What I Learned

This project helped me practice:

* Building workflows with n8n
* Working with APIs
* Understanding JSON responses
* Passing data between workflow steps
* Connecting AI models to automated workflows
* Processing and filtering API results
* Designing user input forms
* Automating email delivery
* Thinking about how AI can improve traditional API-based applications

🔐 Security

API keys, credentials, passwords, tokens, and private webhook information are not included in this repository.

Any credentials required to reproduce the workflow should be configured through environment variables or n8n’s credential system.

🚧 Future Improvements

Planned improvements include:

* Better ranking based on user preferences
* More search categories
* Map-based visualization
* Distance and travel-time comparison
* User preference history
* Additional delivery channels
* A standalone web interface
* More advanced AI recommendation logic
* Rebuilding parts of the workflow using Python/JavaScript

👨‍💻 Project Status

Current status: Working prototype

The project is being developed as a practical AI automation portfolio project, with additional features planned.

⸻

Built with n8n + APIs + AI