🔍 Multimodal Search Engine (Text + Images) using CLIP

Semantic search inside PDFs — across both text and images — using OpenAI’s CLIP model.

A real AI-powered search engine for any document.
Built as part of my #365DaysOfAI challenge — Day 16.

✨ What It Does

Upload any PDF → search with a natural query → get semantically matched results from:

  📄 Text chunks

  🖼 Images extracted from the PDF

No keyword matching. No manual tagging.
Just meaning-powered retrieval using OpenAI’s CLIP embeddings and cosine similarity.
💡 Example Queries

  “scanning garments”

  “robot sewing fabric”

  “privacy concerns in AI”

  “chart about revenue”

  “diagram of neural network”

📦 Features

✅ Extract text chunks from any PDF
✅ Extract all images with page metadata
✅ Generate CLIP embeddings for both text & images
✅ Cosine similarity search with your query
✅ Clean Streamlit UI to view & filter results
📁 Folder Structure

multimodal_search/
├── data/
│ ├── source.pdf ← your input PDF
│ └── images/ ← extracted images
├── embeddings/ ← stores .pkl embeddings
│ ├── text.pkl
│ └── images.pkl
├── search.py ← runs preprocessing
├── streamlit_app.py ← Streamlit UI
└── utils.py ← core logic (CLIP, extraction, search)
🚀 Quick Start

  Clone this repo:

git clone https://github.com/yourusername/multimodal-search-ai.git
cd multimodal-search-ai

  Create a virtual environment (optional but recommended):

python -m venv .venv
.venv\Scripts\activate  # Windows

  Install dependencies:

pip install -r requirements.txt

  Place your PDF at:

📄 data/source.pdf

  Run preprocessing:

python search.py

  Launch the Streamlit UI:

streamlit run streamlit_app.py

![Screenshot 2025-06-25 123837](https://github.com/user-attachments/assets/7e3909ab-35e9-41a7-b2ed-eff29e2efbac)
![Screenshot 2025-06-25 123849](https://github.com/user-attachments/assets/7b612a59-c760-41d2-8285-eca0d844addf)
![Screenshot 2025-06-25 123901](https://github.com/user-attachments/assets/2aba7fcc-7453-46e1-9307-14353aeb0433)


(You can replace these placeholder images with your own screenshots)
🧠 Built With

  OpenAI CLIP

  PyMuPDF (fitz) for PDF parsing

  Streamlit for UI

  sklearn + torch for embeddings and similarity

🧵 TailorAI Demo

I tested this project on a tailoring tech PDF (TailorAI) to simulate real-world fashion search use cases.

Examples:

  "Scan garments" → returned body scanning text

  "Fabric cutting robot" → returned diagrams + automation logic

  "Data privacy" → matched security policy lines

This could be a game-changer for fashion tech, education, or legal documents!
🌍 Use Cases

   📚 Semantic search in academic papers

   🏛 Legal & policy docs

  🧵 Fashion design or AI tailoring

    🧠 E-learning & training materials

    📸 Design/image-based reports

📄 License

MIT License
