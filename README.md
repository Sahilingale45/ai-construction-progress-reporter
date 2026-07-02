# ai-construction-progress-reporter
A real-time automation blueprint that captures construction form webhooks, analyzes site photos using AI, generates formatted progress reports, and emails summaries via Gmail.
# AI-Powered Construction Site Progress Reporter

This repository houses an automated workflow blueprint designed to capture field form submissions, analyze construction site imagery with AI Vision, compile professional text reports, and email them directly to project stakeholders.

## 🚀 How It Works
1. **Trigger (Construction Form Webhook):** Instantly captures inbound form data and uploaded site image links straight from the field via a live HTTP POST webhook endpoint.
2. **Visual Analysis (Analyze Site Photos):** Feeds the site images to an AI vision module to automatically analyze structural progress, material layouts, or safety compliance.
3. **Drafting (Generate Progress Report):** Takes the visual insights alongside form data to write a detailed textual progress summary.
4. **Data Formatting (Parse JSON Report & Format Email):** Converts the AI text report into a clean JSON structure and maps those variables neatly into a polished email body layout.
5. **Delivery (Send Report Email):** Routes the finalized report text to an integrated Gmail node, sending the summary out to clients or managers immediately.

## 📦 What's Included
* `/blueprints/ai-construction-progress-reporter.json`: The complete structural workflow configuration blueprint file.

## 🔧 Setup Instructions
1. Open your automation workflow dashboard workspace.
2. Create a new scenario project, open the tool properties panel, and select **Import Blueprint**.
3. Upload the `.json` blueprint file from this repository.
4. Set up your connections and parameters:
   * **Webhook Trigger:** Copy the generated webhook URL and link it to your field form tool (e.g., Jotform, Typeform, or a custom application).
   * **AI Modules:** Connect your preferred LLM provider (e.g., Google Gemini AI or OpenAI) with your workspace API Key to process both the image analysis and report generation steps.
   * **Gmail Module:** Authorize access to your business mail handle and configure your stakeholder recipient distribution list.
5. Save your current version and toggle the main automation runtime switch to **ON**.
