**Automated Email System with Dynamic File Attachments.**

This repository contains a comprehensive solution for automating the process of sending customized emails with dynamic file attachments. The system is designed to handle various formats such as PDFs (invoices) and Excel files, ensuring seamless communication between the sender and multiple recipients. The main functionalities are designed for businesses dealing with invoice management, customer interaction, and automated mailing operations.

**Key Features:**

1. **Automated Email Generation**:
Sends personalized emails to multiple recipients.
Retrieves recipient details (email addresses, customer names) from a provided Excel sheet.
Generates an email body dynamically with customizable content, including a summary table based on the recipient’s data.

2. **Dynamic File Attachments**:
Automatically attaches PDF invoices and Excel files based on the corresponding customer’s records.
Uses invoice numbers and customer IDs to locate and attach the correct files from extracted ZIP archives.
Supports multiple types of attachments (invoices, Excel files, and images) and additional file attachments if needed.

3. **ZIP File Management**:
Extracts contents from ZIP files containing invoices and Excel files.
Ensures all files are correctly categorized and mapped to their respective customers before being attached to emails.

4. **Rich HTML Email Content**:
Creates visually appealing email bodies using HTML.
Embedded QR codes within emails, offering convenient access to additional information or actions.
Includes tables of invoice details for each customer, formatted with customizable styles.

5. **Multi-Language Support**:
Generates email content in multiple languages (e.g., Tamil, Telugu, Kannada, Malayalam) for personalized regional communication.
Ensures that language-specific content is clear, concise, and professionally formatted.

6. **Configurable Email Settings**:
Email settings (SMTP server, port, credentials) are customizable and securely handled.
CC and BCC email addresses can be hardcoded or dynamically configured based on business needs.

7. **Secure & Scalable**:
Uses Python’s smtplib for secure email transmission over TLS.
Can handle large datasets with multiple customers and a variety of attachments efficiently.

8. **Error Handling & Debugging**:
Includes comprehensive error handling for missing files, email transmission failures, and PDF/Excel parsing issues.
Outputs logs for debugging, showing detailed information about each file extraction and email process.

9. **Modular Code Structure**:
Designed with modular functions to ensure ease of modification and scalability.
Can be adapted to integrate with other types of files, email services, or new features as business needs evolve.

**Use Cases**:

- **Invoice Delivery**: Automatically emails monthly invoices to customers, attaching PDF invoices and related financial statements.
- **Customer Communication**: Sends customized reports and summaries based on customer data stored in Excel files.
- **Payment Reminders**: Sends payment reminders or outstanding balance summaries with dynamically generated content and attachments.

**Technical Details:**
**Language**: Python
**Key Libraries**:
**os, zipfile:** For file and ZIP management.
**smtplib, email.mime:** For email construction and sending.**
pandas:** For data manipulation and Excel processing.
**PyPDF2:** For reading and extracting text from PDF files.
**Dependencies:** Install dependencies using pip install -r requirements.txt
