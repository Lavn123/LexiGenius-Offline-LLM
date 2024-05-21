# LexiGenius

#Introduction to Lexi Genius

Lexi Genius is a powerful offline tool designed to summarize PDF documents efficiently. Leveraging advanced natural language processing (NLP) technologies, this application provides accurate and concise summaries of PDF files while maintaining privacy by running locally on your machine. It's an ideal tool for professionals, students, and anyone who needs to handle large volumes of text.

# How Lexi Genius Works

1. Model and Tokenizer Loading: 
   Lexi Genius uses the `T5-small` model from Hugging Face's Transformers library. This model is known for its efficiency in text generation tasks, including summarization. The model and tokenizer are loaded into the application to process and summarize text.

2. File Loading and Preprocessing:
   Users can upload PDF files, which the application processes using the `PyPDFLoader`. This component reads the PDF, splits it into manageable chunks using the `RecursiveCharacterTextSplitter`, and prepares these chunks for summarization.

3. Text Summarization:
   The summarization function encodes the input text, generates a summary using the T5 model, and decodes the output. This process ensures that each chunk of text from the PDF is summarized effectively.

4. Displaying the PDF:
   Lexi Genius can display the uploaded PDF directly within the app. This is achieved by embedding the PDF in an iframe using base64 encoding, allowing users to view the document while it is being processed.

5. User Interface and Interaction:
   The application is built using Streamlit, providing a simple and interactive user interface. Users can upload their PDF files, adjust summarization parameters, and generate summaries with a click of a button. The app includes features like file upload, parameter adjustment, and a progress bar to enhance the user experience.

#Usage

- Upload a PDF: Use the file uploader to select a PDF file for summarization.
- Adjust Parameters: Customize the maximum summary length using the slider provided.
- Generate Summary: Click the "Generate Summary" button to start the summarization process. The application will display the PDF and show a progress bar while summarizing.
- View Summary: Once the summarization is complete, the summary will be displayed within the app.

Lexi Genius* is designed to make the task of summarizing large PDF documents easy and efficient, providing users with quick insights and saving valuable time.
