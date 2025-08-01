# CodeAlpha FAQ Chatbot

An intelligent, user-friendly web-based FAQ chatbot that answers common questions using a combination of keyword matching and AI-powered fallback responses.

## Features

- **Custom FAQ Matching:** Uses text preprocessing and cosine similarity to find the best matches in a predefined FAQ database.
- **AI-Powered Fallback:** If no confident FAQ answer is found, queries are forwarded to OpenAI GPT-3.5 Turbo API for smart, context-aware replies.
- **Responsive UI:** Built with clean HTML, CSS, and JavaScript, featuring a modern, minimalist chat interface that works on all screen sizes.
- **Typing Indicator:** Mimics real chatbot behavior with animated typing dots for enhanced realism.
- **Suggested Questions:** Quick-access chips to popular FAQs for faster interaction.
- **Confidence Scores:** Displays confidence levels for FAQ responses to indicate answer reliability.

## Usage

1. Open `index.html` in a modern web browser.
2. Type your question in the input box and press **Enter** or click the send button.
3. See instant responses either from the FAQ database or AI-generated answers.
4. Click on the suggested question chips to quickly ask common FAQs.

## FAQ Database

The chatbot comes preloaded with common FAQs about business hours, support contacts, services offered, account creation, payment methods, refunds, project completion times, and technical support.

## Requirements

- Internet connection (for OpenAI API fallback)
- Modern web browser

## Configuration

- Replace the placeholder OpenAI API key in the script with your own key:
  
const API_KEY = 'YOUR_OPENAI_API_KEY_HERE';


## How It Works

- User input is preprocessed to normalize and tokenize text.
- Similarity scores are calculated between input and FAQ question/keyword sets using cosine similarity.
- If the best FAQ match exceeds a confidence threshold (30%), the chatbot returns the FAQ answer.
- Otherwise, the input is sent to OpenAI’s GPT-3.5 Turbo model with the FAQ context for an AI-generated response.
- Responses are displayed with appropriate UI flair, including confidence scores for FAQ matches.

## Folder Structure

- `index.html` – Main chatbot interface and logic (front-end only).
- CSS and JavaScript are embedded within `index.html` (can be separated if desired).

## Future Improvements

- Add backend integration to manage FAQs dynamically.
- Store chat history in local storage or backend.
- Enhance NLP with advanced ML models for better FAQ matching.
- Expand chatbot capabilities beyond FAQs.

## Author

Dhanush Shenoy H

---

For any questions or support, please contact: dshenoyh@gmail.com
