# Resume Shortlisting Program

This program is designed to scan a selected directory, extract information from PDF resumes, and summarize the content using a Transformer model from Hugging Face. The extracted information is then saved to a CSV file for easy shortlisting.

## Libraries Used

1. **tkinter**: A GUI library for selecting the directory.
2. **transformers**: A Hugging Face library for summarizing the text.
3. **csv**: A library for converting data into CSV format.
4. **PyPDF2**: A library for reading PDF files.
5. **os**: A library for handling directories and files.
6. **re**: A library for regular expressions.

## Functions

### file\_dialog()

This function opens a file dialog to select a directory containing PDF resumes. It then:

1. Scans the directory for PDF files.
2. Initializes the Transformer pipeline for text summarization.
3. Defines regular expressions for extracting emails and phone numbers.
4. Traverses the list of PDF files, extracting metadata, text, and summarizing the content.
5. Saves the extracted information to a CSV file.

## How to Use

1. Run the program.
2. Select the directory containing the PDF resumes.
3. The program will scan the directory, extract information, summarize the content, and save it to a CSV file named "resume.csv".

## Note

The program assumes that each PDF contains only one page. If a PDF has multiple pages, the program may not work as expected. Additionally, the program uses the T5 base model for summarization, which may not always produce perfect summaries.
