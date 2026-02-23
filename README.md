AI Invoice Document Extractor with Visual Annotation

An end-to-end Document Intelligence pipeline that automatically extracts structured information from invoice PDFs and generates visually annotated outputs for explainable verification.

This project demonstrates practical integration of multimodal LLMs + PDF rendering to build a reliable invoice automation system suitable for real-world finance and operations workflows.


System Architecture

Invoice PDF
→ Gemini Flash (Multimodal Extraction)
→ Structured Schema Validation
 → Bounding Box Mapping
 → PyMuPDF Renderi
 → Annotated PDF Output

doc-extractor/
│
├── main.py                  # Core extraction + annotation pipeline
├── invoice.pdf              # Sample input
├── invoice_annotated.pdf    # Output with visual bounding boxes
├── .env                     # API key configuration
└── requirements.txt         # Dependencies


Tech Stack:--

Python

Gemini Flash (Multimodal LLM)

PyMuPDF (PDF rendering & annotation)

Pydantic (Schema validation)

python-dotenv (Environment management)


Setup & Run
1. Install dependencies
pip install pymupdf python-dotenv google-genai pydantic

2. Configure API key
Create .env
GEMINI_API_KEY=your_key_here

3. Run project
python main.py

4. Output
invoice_annotated.pdf

           
