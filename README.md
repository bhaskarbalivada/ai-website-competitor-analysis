 # AI-Powered Website Competitor Analysis

An AI-powered website analysis and competitive intelligence workflow built using **n8n and Google Gemini**. It accepts a website URL through a chat interface, analyzes the website's business and services, and generates insights about its top three competitors.

## 🚀 Project Overview

This project automates the process of understanding a website and identifying its competitors. Instead of manually researching a company's offerings and competitive landscape, users can submit a website URL and receive an AI-generated analysis report.

The workflow uses two AI Agent nodes powered by Google Gemini to perform website analysis and competitor analysis sequentially.

## ✨ Features

- **Website Overview:** Identifies the website's purpose, industry, and core business.
- **Service and Product Analysis:** Summarizes services, products, features, benefits, and available pricing information.
- **Target Audience Analysis:** Identifies the intended users and customers.
- **Business Model Analysis:** Examines potential revenue models based on available information.
- **Top 3 Competitors:** Identifies three relevant direct or indirect competitors.
- **Competitor Comparison:** Compares services, pricing, target audiences, features, and differentiators.
- **Competitive Insights:** Highlights potential strengths, limitations, and opportunities for improvement.
- **Chat-Based Interaction:** Allows users to submit website URLs through the n8n chat interface.

## 🔄 Workflow Architecture

The workflow consists of the following nodes:

1. **When Chat Message Received** — Receives the user's message containing the website URL.
2. **AI Agent** — Analyzes the website's overview, products, services, target audience, business model, and features.
3. **Google Gemini Chat Model** — Powers the first AI Agent.
4. **AI Agent1** — Processes the initial analysis and generates competitor research and comparison insights.
5. **Google Gemini Chat Model1** — Powers the second AI Agent.

### Workflow Flow

`User Input → Website Analysis → Competitor Analysis → Final Report`

## 🛠️ Technologies Used

- **n8n** — Workflow automation platform
- **Google Gemini** — AI-powered website and competitor analysis
- **AI Agent Nodes** — Multi-stage analysis and report generation
- **Chat Trigger** — User input through a conversational interface

## ⚙️ Setup and Installation

1. Install or access n8n.
2. Create a new workflow.
3. Import the `website competetors.json` workflow file.
4. Configure your Google Gemini API credentials in n8n.
5. Verify that both Google Gemini Chat Model nodes use the correct credentials.
6. Open the workflow's chat interface.
7. Enter a website URL to request an analysis.
8. Review the generated website report and competitor comparison.

## 💡 Example Input

`https://example.com`

## 📊 Expected Output

The workflow is designed to produce:

- Website overview and business category
- Main products and services
- Target audience and business model
- Three relevant competitors
- Competitor comparison and differentiators
- Competitive insights and improvement opportunities

The exact level of detail depends on the information available to the AI agents and their configured output instructions.

## ⚠️ Limitations

- The workflow's accuracy depends on the information available to the AI models.
- Competitor details and pricing should be independently verified.
- The exported workflow does not contain a dedicated web-search or website-crawling node. Therefore, verified live research is not guaranteed by the current workflow alone.
- Both AI Agent system prompts request output limited to 100 words in a tabular representation, which may restrict the detail of the final report.

## 🔮 Future Improvements

- Integrate a web-search API to retrieve current competitor information.
- Add website scraping or crawling for more reliable website content extraction.
- Include source URLs and citations for competitor claims.
- Generate downloadable PDF or HTML reports.
- Add structured output validation and error handling.

## 🎯 Use Cases

- Startup competitor research
- Business and market analysis
- Website service discovery
- Preliminary competitive intelligence
- Product and service benchmarking

## 📄 License

Choose an appropriate open-source license before distributing or reusing this project.

---

**Built with n8n and Google Gemini.**
