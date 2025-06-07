# TakeForm Backend

Backend service for the TakeForm MVP: transforms 2D architectural drawings (PDFs/images) into 3D visualizations and automated quantity takeoffs.

## Directory Structure

```
takeform-backend/
├── app/
│   ├── __init__.py
│   ├── main.py              # FastAPI app
│   ├── parser/
│   │   ├── __init__.py
│   │   ├── pdf_parser.py    # Handles PDF via PyMuPDF & OCR
│   │   ├── image_parser.py  # Handles scans/images
│   │   ├── dxf_parser.py    # Handles DXF with ezdxf
│   └── utils/
│       └── preprocessing.py # OpenCV functions, shared logic
├── tests/
│   ├── test_pdf_parser.py
│   └── test_dxf_parser.py
├── requirements.txt
├── .gitignore
└── README.md
```