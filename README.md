# ocr_anamnese

This project is an automated pipeline designed to bridge the gap between physical medical records and digital health systems. It focuses on converting images of anamnesis forms—often handwritten or printed—into structured, actionable digital reports.

The workflow is divided into three core stages:

Image Optimization & Extraction: Using OpenCV, the system applies pre-processing filters (such as sharpening and noise reduction) to enhance the legibility of the document. Then, EasyOCR scans the image to extract raw text data from the medical forms.

Intelligent Data Interpretation: Raw OCR output can often be fragmented or disorganized. To solve this, the project integrates Llama 3 (via Ollama) to act as a clinical interpreter. The AI analyzes the extracted text, understands the medical context, and organizes the information into logical sections like patient identification, symptoms, and clinical history.

Automated Reporting: Finally, the system uses tools like WeasyPrint and Pandoc to transform the AI’s analysis into a professional, formatted PDF report.

Essentially, the tool replaces manual data entry, providing healthcare professionals with a searchable, digitized version of patient records while maintaining clinical structure.
