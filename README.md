<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>
<body>

<header>
  <h1>Real-Time Face Mask Detection</h1>
  <p> This project implements a real-time face mask detection system using <b>Deep Learning</b> and 
      <b>Transfer Learning (MobileNetV2)</b>. The goal is to classify whether a person is wearing a mask or not, 
      using webcam/video streams as well as static images.<br><br>
   I've made it super simple – no local setup, no CUDA and cuDDN, no complicated pip/conda installations. You just need Google Colab + 3 notebooks</p><br>

   <p>
      This project implements a <strong>real-time face mask detection system</strong> 
      using <code>TensorFlow</code>, <code>Keras</code>, and <code>OpenCV</code>. 
      The model classifies whether a person is wearing a mask or not from a live camera feed.
    </p>
   <p>
      The system is trained on a combined dataset of multiple Kaggle datasets (~18k images) to improve accuracy and robustness. 
      The project was developed and tested in <b>Google Colab</b> for easy accessibility and GPU acceleration.
    </p>
</header>

<main>


<section>
    <h2>🚀 Importance</h2>
    <ul>
      <li>Enforcing safety protocols in public places</li>
      <li>Preventing the spread of infectious diseases</li>
      <li>Supporting authorities with low-cost, scalable solutions</li>
    </ul>
  </section>

   <section>
    <h2>📂 Dataset</h2>
    <ul>
      <li>Created by combining multiple Kaggle datasets (Mask / No Mask)</li>
      <li>~18,500 images used</li>
      <li>Preprocessing: resized to 224x224, normalized, and augmented (flips, rotations, zoom)</li>
    </ul>
  </section>

  <h2>📌 Features</h2>
    <ul>
      <li>Real-time face mask detection using webcam</li>
      <li>Trained with MobileNetV2 for high accuracy</li>
      <li>Supports both mask and no-mask classification</li>
      <li>Lightweight and fast for real-time deployment</li>
    </ul>

  <section>
     <h2>🧠 Model (MobileNetV2)</h2>
    <p><b>Base Model:</b> Pre-trained MobileNetV2 on ImageNet</p>
    <p><b>Custom Layers:</b></p>
    <ul>
      <li>GlobalAveragePooling2D</li>
      <li>BatchNormalization</li>
      <li>Dropout (0.5 and 0.3)</li>
      <li>Dense (ReLU + Softmax for binary classification)</li>
    </ul>
    <p><b>Training Strategy:</b></p>
    <ul>
      <li>Phase 1: Train top layers with frozen base</li>
      <li>Phase 2: Fine-tune deeper layers with a lower learning rate</li>
    </ul>
    <p><b>Optimizations:</b> EarlyStopping, ReduceLROnPlateau, ModelCheckpoint</p>
  </section>

    

  <section id="how-to-run">
  <h2 style="color:#111; margin-top:0;">⚡ How to Run (Easiest Method)</h2>

  <ol style="line-height:1.8; color:#333; font-size:16px;">
    <li><strong>Download</strong> the <code>.ipynb</code> files from this repo (click file → Download → save to your system).</li>
    <li><strong>Open</strong> <a href="https://colab.research.google.com/" target="_blank" style="color:#0066cc; text-decoration:none;">Google Colab</a>.</li>
    <li><strong>Upload</strong> each notebook (<code>.ipynb</code>) one by one into Colab (File → Upload notebook).</li>
    <li><strong>Run all cells</strong> (use <code>Shift + Enter</code> for each cell). Colab will automatically:
      <ul style="margin-top:8px; margin-bottom:8px;">
        <li>Install required libraries (TensorFlow, OpenCV, etc.).</li>
        <li>Download pretrained models if needed.</li>
        <li>Prepare the runtime and GPU (if you enable GPU).</li>
      </ul>
    </li>
    <li style="margin-top:6px;"><strong>Done ✅</strong> — you can train, test, or run the real-time demo without installing CUDA, Python, or extra packages locally.</li>
  </ol>

  <p style="background:#f0f8ff; padding:10px; border-radius:6px; color:#055160; margin-top:12px;">
    <strong>Tip:</strong> In Colab set Runtime → Change runtime type → GPU for faster training (optional).
  </p>
</section>


  <section class="section">
    <h2>📂 Project Structure</h2>
    <pre><code>📦 Real Time Face Mask Detection
 ┣ 📜 Face Mask Detection DeepLearning.ipynb
 ┣ 📜 RealTimeDetection.ipynb
 ┣ 📜 Using the trained model.py
 ┣ 📂 dataset
</code></pre>
  </section>

  <section class="section">
    <h2>📊 Dataset</h2>
    <p>
      The model is trained on a dataset of images consisting of two classes:
    </p>
    <ul>
      <li>With Mask 😷</li>
      <li>Without Mask 🙂</li>
    </ul>
  </section>

  <section class="section">
    <h2>🧠 Model</h2>
    <p>
      The detection is based on a <strong>Convolutional Neural Network (CNN)</strong> 
      built using TensorFlow & Keras. The model is trained on thousands of face images to 
      classify mask/no-mask with high accuracy.
    </p>
  </section>

  <section class="section">
    <h2>📸 Demo</h2>
    <p>
      Example of real-time mask detection output:
    </p>
    <img src="demo.png" alt="Demo Output" width="600">
  </section>

  <section class="section">
    <h2>🤝 Contributing</h2>
    <p>
      Contributions, issues, and feature requests are welcome!  
      Feel free to fork this repo and submit a pull request.
    </p>
  </section>

  <section class="section">
    <h2>📜 License</h2>
    <p>
      This project is licensed under the <strong>MIT License</strong>.
    </p>
  </section>

</main>

<footer>
  <p>Made with ❤️ using TensorFlow & OpenCV</p>
</footer>

</body>
</html>
