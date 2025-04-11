# MultiLanguage Invoice Extractor

Demo Video Link :- https://drive.google.com/file/d/1GCkRiqpqZ1s7DgpOWS2LexbC8GX6QhEa/view?usp=sharing

This is a Streamlit-based web application that uses **Google Gemini Pro Vision** to analyze and extract information from **invoice images** in multiple languages. Just upload an image and ask your question—the AI will handle the rest!

---

## Features

- Upload invoice images in `.jpg`, `.jpeg`, or `.png` format
- Supports invoices in **multiple languages**
- Powered by **Gemini Pro Vision** (Google Generative AI)
- Extracts totals, item details, dates, invoice numbers, and more
- Accepts **custom user prompts** to extract specific information
- Clean and interactive user interface built with Streamlit

---

## Tech Stack

- **Python**
- **Streamlit** – Web interface
- **Google Generative AI (Gemini Pro Vision)**
- **Pillow (PIL)** – Image processing
- **python-dotenv** – To manage environment variables securely

---

## Project Structure

```
MultiLanguage-Invoice-Extractor/
│
├── .env                 # API key stored here (not shared publicly)
├── app.py              # App application script
├── requirements.txt     # List of Python dependencies
├── README.md            # Project documentation
```

---

## Getting Started

### 1. Clone the Repository


### 2. Set Up Environment Variables

Create a `.env` file in the project root and add your Google API key:

```
GOOGLE_API_KEY=your_api_key_here
```

### 3. Install Dependencies

It's recommended to use a virtual environment:

```bash
pip install -r requirements.txt
```

### 4. Run the Streamlit App

```bash
streamlit run main.py
```

---

## How It Works

1. User uploads an invoice image.
2. The image is processed and converted to a format that Gemini can understand.
3. User enters a custom prompt/question.
4. The image and prompt are sent to Gemini Pro Vision model.
5. AI returns a response based on the content of the image and the prompt.

---

## Example Prompts

- "What is the total amount on this invoice?"
- "List all the items and their prices."
- "Extract the invoice number and date."
- "Translate the invoice to English & Telugu and summarize."

---

## Future Improvements

- Export extracted data to CSV or Excel
- Add PDF invoice support
- Add language translation and detection features
- Improve error handling and user instructions
