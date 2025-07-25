🧠 Face Friend Finder – Face Recognition Web App

A modern face recognition web application built with **React**, **TypeScript**, and **face-api.js**. This app provides real-time face detection, expression analysis, and demographic estimation in a sleek and responsive UI.


🚀 Features

* 👤 **Face Detection** – Detect multiple faces in uploaded images
* 😊 **Expression Analysis** – Recognize emotions (happy, sad, angry, surprised, etc.)
* 📊 **Age & Gender Estimation** – Estimate age and gender of detected faces
* ⚡ **Real-time Processing** – Fast detection using TinyFaceDetector
* 🎨 **Modern UI** – Responsive interface with AI-themed design
* 💾 **Download Results** – Save analyzed images with detection overlays

🛠️ Technology Stack

| Category      | Tools Used                         |
| ------------- | ---------------------------------- |
| Frontend      | React 18, TypeScript, Tailwind CSS |
| AI / ML       | face-api.js                        |
| UI Components | shadcn/ui (custom themed)          |
| Build Tool    | Vite                               |
| Routing       | React Router DOM                   |

---

⚙️ Getting Started

🔍 Prerequisites

* Node.js (v16 or higher)
* npm or yarn

🧰 Installation Steps

1. **Clone the repository**:

   ```bash
   git clone https://github.com/your-username/face-friend-finder.git
   cd face-friend-finder
   ```

2. **Install dependencies**:

   ```bash
   npm install
   ```

3. **Download face-api.js models**:

   * Go to: [face-api.js models](https://github.com/justadudewhohacks/face-api.js/tree/master/weights)
   * Download the following files into `public/models/`:

     ```
     tiny_face_detector_model-weights_manifest.json
     tiny_face_detector_model-shard1
     face_landmark_68_model-weights_manifest.json
     face_landmark_68_model-shard1
     face_expression_model-weights_manifest.json
     face_expression_model-shard1
     age_gender_model-weights_manifest.json
     age_gender_model-shard1
     ```

4. **Start development server**:

   ```bash
   npm run dev
   ```

5. Visit `http://localhost:8080` in your browser

🧪 How to Use

1. Upload an image (click or drag & drop)
2. Wait for face detection and analysis
3. View bounding boxes, expressions, age & gender
4. Download the result with overlays

📁 Supported Image Formats

* PNG
* JPEG / JPG
* GIF
* BMP
* WebP

 👓 Face Detection Capabilities

* **Face Detection** – Bounding boxes for multiple faces
* **Facial Landmarks** – 68-point detection
* **Expression Recognition** – Emotions like happy, sad, neutral
* **Age Estimation**
* **Gender Classification**

🧩 Project Structure

```
src/
├── components/
│   ├── ui/                   # shadcn/ui components
│   ├── FaceRecognition.tsx   # Main detection UI
│   ├── ImageUpload.tsx       # Upload functionality
│   └── FaceDetectionResults.tsx # Display results
├── hooks/
│   └── useFaceDetection.ts   # Custom detection logic
├── pages/
│   └── Index.tsx             # Landing page
└── styles/
    └── index.css             # AI-themed global styles
```

 🎨 Customization

* Tailwind themes and CSS variables defined in:

  * `index.css`
  * `tailwind.config.ts`

You can modify color palettes, animations, and layout styles as needed.

⚡ Performance Notes

* On-demand model loading
* TinyFaceDetector ensures fast processing
* Efficient rendering using `<canvas>`

🌐 Browser Support

* ✅ Chrome (Recommended)
* ✅ Firefox
* ✅ Safari
* ✅ Edge

 🤝 Contributing

1. Fork the repo
2. Create a new branch
3. Make your changes
4. Push your changes
5. Submit a pull request


📜 License
This project is licensed under the **MIT License** – see the `LICENSE` file for details.

 🙌 Acknowledgments
* [face-api.js](https://github.com/justadudewhohacks/face-api.js) – Face detection engine
* [shadcn/ui](https://ui.shadcn.com/) – Beautiful UI components
* [Tailwind CSS](https://tailwindcss.com/) – Utility-first CSS framework
