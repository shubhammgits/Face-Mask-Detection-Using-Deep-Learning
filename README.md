<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>
<body>

<header>
  <h1>Real-Time Face Mask Detection</h1>
  <p>A Deep Learning based project using TensorFlow & OpenCV <br>
   I've made it super simple – no local setup, no CUDA and cuDDN, no complicated pip/conda installations. You just need Google Colab + 3 notebooks</p>
</header>

<main>

  <section class="section">
    <h2>📌 Overview</h2>
    <p>
      This project implements a <strong>real-time face mask detection system</strong> 
      using <code>TensorFlow</code>, <code>Keras</code>, and <code>OpenCV</code>. 
      The model classifies whether a person is wearing a mask or not from a live camera feed.
    </p>
  </section>

  <h2>📌 Features</h2>
    <ul>
      <li>Real-time face mask detection using webcam</li>
      <li>Trained with MobileNetV2 for high accuracy</li>
      <li>Supports both mask and no-mask classification</li>
      <li>Lightweight and fast for real-time deployment</li>
    </ul>

  <section id="how-to-run" style="font-family: Arial, sans-serif; max-width:900px; margin:30px auto; background:#fff; padding:20px; border-radius:10px; box-shadow:0 6px 18px rgba(0,0,0,0.06);">
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
    <strong>Tip:</strong> In Colab set Runtime → Change runtime type → GPU for faster training (optional).
  </p>
</section>


  <section class="section">
    <h2>🚀 Usage</h2>
    <p>Run the following command to start real-time mask detection:</p>
    <pre><code>python RealTimeDetection.py</code></pre>
    <p>
      The webcam will open and display real-time detection results.
      <ul>
        <li><span style="color: green;">Green Box → Person is wearing a mask ✅</span></li>
        <li><span style="color: red;">Red Box → Person is not wearing a mask ❌</span></li>
      </ul>
    </p>
  </section>

  <section class="section">
    <h2>📂 Project Structure</h2>
    <pre><code>📦 RealTimeDetection
 ┣ 📜 RealTimeDetection.ipynb
 ┣ 📜 RealTimeDetection.py
 ┣ 📜 requirements.txt
 ┣ 📂 dataset
 ┗ 📂 models
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
