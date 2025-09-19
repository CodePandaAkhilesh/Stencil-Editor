# Stencil Editor (React + Fabric.js + Redux + Tailwind)
1. A Canvas-based Stencil Editor built with React, Vite, Redux, and Fabric.js.
2. It allows users to:

   - Upload an image.

   - Drag & drop it into a predefined stencil (photo frame).

   - Move, zoom, and reset the image inside the stencil.

🚀 Getting Started

1. Clone the repository
   git clone https://github.com/CodePandaAkhilesh/Stencil-Editor.git
   cd Stencil-Editor

2. Install dependencies
   npm install
   npm install fabric @reduxjs/toolkit react-redux
   npm install -D tailwindcss postcss autoprefixer
   npx tailwindcss init -p

3. Run the development server
   npm run dev

4. Upload an image via the left Uploads panel. Use Zoom +/– to zoom inside the stencil, drag image to reposition, use Reset to restore.


📂 Project Structure

   Stencil-Editor/
   ├── public/              # Static assets
   ├── src/
   │   ├── components/
   │   │   ├── CanvasEditor.jsx   # Fabric.js canvas + stencil logic
   │   │   ├── LeftPanel.jsx      # Handles uploads & thumbnails
   │   │   ├── Toolbar.jsx        # Zoom, Reset, Undo controls
   │   ├── store/
   │   │   ├── editorSlice.js     # Redux slice for editor state
   │   │   └── store.js           # Redux store setup
   │   ├── App.jsx                # Main layout
   │   ├── main.jsx               # React entrypoint
   │   ├── index.css              # Global styles (Tailwind included)
   ├── index.html
   ├── vite.config.js
   ├── tailwind.config.js
   ├── postcss.config.js
   ├── package.json
   └── README.md
