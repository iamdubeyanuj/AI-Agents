# AI-Agents
# Gradio Career Concierge

A Gradio-powered personal career chatbot that answers questions based on a profile summary and LinkedIn PDF. It can also record contact details and unknown questions via Pushover notifications.

## Features
- Gradio chat UI
- Profile-aware responses (summary + LinkedIn)
- Tool calls to record emails and unknown questions
- Pushover notifications for lead capture

## Setup
1. Create a virtual environment (optional but recommended).
2. Install dependencies:
   - `pip install -r requirements.txt`
3. Create a `.env` file with:
   - `OPENAI_API_KEY`
   - `PUSHOVER_TOKEN`
   - `PUSHOVER_USER`
4. Add your profile assets:
   - `me/summary.txt`
   - `me/linkedin.pdf` (optional; the app will run without it)

## Run
- `python app.py`

## Notes
- If `PUSHOVER_TOKEN` or `PUSHOVER_USER` are missing, Pushover calls will fail.
- Replace the content of `me/summary.txt` with your own summary.
