<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>
<body>

<header>
  <h1>Real-Time Face Mask Detection</h1>
  <p>A Deep Learning-based project using TensorFlow & OpenCV</p>
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

  <section class="section">
    <h2>⚙️ Installation</h2>
    <p>Clone the repository and install the required dependencies:</p>
    <pre><code>git clone https://github.com/your-username/RealTimeDetection.git
cd RealTimeDetection
pip install -r requirements.txt
</code></pre>
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
