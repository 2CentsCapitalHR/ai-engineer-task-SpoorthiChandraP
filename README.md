# ADGM-Compliant Corporate Agent with Document Intelligence

A Streamlit-based tool to review ADGM-related legal documents against a compliance checklist, detect red flags, and produce both JSON reports and reviewed `.docx` files with comments.

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Features
- Upload multiple `.docx` files at once
- Detects document type based on content
- Compares uploaded documents to required ADGM checklist
- Flags common red flags (wrong jurisdiction, missing signature section, etc.)
- Generates:
  - JSON analysis report
  - Reviewed `.docx` files with comments/suggestions
- Download buttons in the UI for all results
- Automatically saves results in `outputs/` folder

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Screenshots

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Folder Structure
``` bash 
adgm_corporate_agent/
│ ├── main.py # Streamlit app
├── requirements.txt # Python dependencies
├── README.md # Project instructions
│ ├── examples/ # Original example documents ("before review")
│ ├── aoa_bad.docx │ └── mou_good.docx
│ ├── outputs/ # Generated outputs ("after review")
│ ├── reviewed_aoa_bad.docx
│ ├── reviewed_mou_good.docx
│ ├── output.json
│ ├── Screenshot 1.png
│ └── Screenshot 2.png
```

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Setup

### 1. Clone the repository or extract the ZIP
```bash
git clone https://github.com/2CentsCapitalHR/ai-engineer-task-SpoorthiChandraP.git
cd ai-engineer-task-SpoorthiChandraP
```

### 2. Create a virtual environment
```bash
python -m venv venv
```

### 3. Activate the virtual environment

On Windows
```bash
venv\Scripts\activate
```

On Mac/Linux
```bash
source venv/bin/activate
```

### 4. Install dependencies
```bash
pip install -r requirements.txt
```

### Run the Application
```bash
streamlit run main.py
```
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

