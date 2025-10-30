🖼️ Gallery Exhibit Defect Detection System
📘 Overview
The Gallery Exhibit Defect Detection System is a Streamlit-based application designed to detect visual defects or surface irregularities in artworks. It helps curators, restorers, and galleries identify potential damage (such as cracks, discoloration, or irregular textures) in digital art images.

This project uses OpenCV and NumPy for image analysis and contour-based defect detection, with interactive visualization and configuration through a modern Streamlit UI.

🚀 Features
🔍 Live Detection: Upload artwork images for real-time AI-based defect detection.

📊 Detection Report: Automatically highlights defects with bounding boxes and confidence scores.

⚠️ Alert Dashboard: Displays critical defect alerts.

🕒 Detection History: (coming soon) Save and view previous detection results.

⚙️ System Settings: Adjust detection sensitivity, enable auto-detection, and filter defect types.

🧠 How It Works
The app compares uploaded artwork images against “damaged” and “undamaged” reference folders.

If an image belongs to the damaged folder, the algorithm dynamically generates defect bounding boxes based on edge and contour detection.

Defects are labeled with:

Type (e.g., Surface Irregularity)

Severity (Low / Critical)

Area

Confidence

The processed image and defect summary are displayed interactively in Streamlit.

🗂️ Project Structure
bash
Copy code
Gallery_Exhibit_Defect_Detection/
│
├── app.py                    # Main Streamlit app
├── README.md                 # Project documentation
├── requirements.txt          # Python dependencies
│
├── unpaired_dataset_art/
│   ├── damaged/              # Damaged artwork images
│   └── undamaged/            # Clean artwork images
│
└── assets/                   # (Optional) Logos or example outputs
🧩 Requirements
Create a requirements.txt file with the following:

nginx
Copy code
streamlit
opencv-python
numpy
pandas
Install dependencies:

bash
Copy code
pip install -r requirements.txt
▶️ Run the App
Clone this repository:

bash
Copy code
git clone https://github.com/yourusername/Gallery-Exhibit-Defect-Detection.git
cd Gallery-Exhibit-Defect-Detection
Launch the Streamlit app:

bash
Copy code
streamlit run app.py
Open the provided local URL in your browser (usually http://localhost:8501).

🧪 Example Usage
Upload a .jpg, .jpeg, or .png image of an artwork.

Click “Analyze for Defects”.

View processed image with bounding boxes and defect summary table.

Critical defects are shown with red alerts.

⚙️ Settings Panel
You can configure:

Detection Sensitivity (slider)

Auto-Detection toggle

Severity filter (“All”, “Critical Only”, “Low Only”)

🧱 Future Enhancements
🧭 Machine learning-based defect classification (CNN or autoencoder)

💾 Save detection history to a database (SQLite or CSV)

🧠 Model explainability dashboard

📩 Automated alert notifications (email or SMS)

🧑‍💻 Author
Abhinav P
AI for Art Restoration — 2025
💡 Passionate about combining computer vision and cultural heritage preservation.
