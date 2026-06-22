<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>House Price Prediction - README</title>
  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; }
    body {
      font-family: 'Segoe UI', sans-serif;
      background: #f4f6f9;
      color: #333;
      padding: 30px 20px;
    }
    .container {
      max-width: 850px;
      margin: auto;
      background: white;
      border-radius: 12px;
      box-shadow: 0 4px 20px rgba(0,0,0,0.08);
      overflow: hidden;
    }
    .header {
      background: linear-gradient(135deg, #1a5276, #2e86c1);
      color: white;
      padding: 40px 30px;
      text-align: center;
    }
    .header h1 { font-size: 2em; margin-bottom: 8px; }
    .header p { font-size: 1em; opacity: 0.9; }
    .badges {
      display: flex;
      flex-wrap: wrap;
      gap: 10px;
      justify-content: center;
      margin-top: 16px;
    }
    .badge {
      background: rgba(255,255,255,0.2);
      border: 1px solid rgba(255,255,255,0.4);
      border-radius: 20px;
      padding: 4px 14px;
      font-size: 0.85em;
    }
    .content { padding: 30px; }
    .section { margin-bottom: 30px; }
    .section h2 {
      font-size: 1.2em;
      color: #1a5276;
      border-left: 4px solid #2e86c1;
      padding-left: 12px;
      margin-bottom: 14px;
    }
    .section p { line-height: 1.7; color: #444; }
    .steps {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
      gap: 14px;
      margin-top: 10px;
    }
    .step {
      background: #eaf4fb;
      border-radius: 10px;
      padding: 16px;
      text-align: center;
    }
    .step .icon { font-size: 1.8em; margin-bottom: 8px; }
    .step h4 { color: #1a5276; font-size: 0.95em; margin-bottom: 4px; }
    .step p { font-size: 0.85em; color: #555; }
    .tech-grid {
      display: flex;
      flex-wrap: wrap;
      gap: 10px;
      margin-top: 10px;
    }
    .tech-tag {
      background: #1a5276;
      color: white;
      border-radius: 20px;
      padding: 6px 16px;
      font-size: 0.88em;
    }
    .dataset-box {
      background: #f0f9f0;
      border: 1px solid #a9dfbf;
      border-radius: 10px;
      padding: 16px 20px;
    }
    .dataset-box p { margin-bottom: 6px; font-size: 0.95em; }
    .dataset-box span { font-weight: bold; color: #1e8449; }
    .algo-list { list-style: none; margin-top: 10px; }
    .algo-list li {
      padding: 10px 14px;
      background: #fef9e7;
      border-left: 4px solid #f4d03f;
      border-radius: 6px;
      margin-bottom: 8px;
      font-size: 0.95em;
    }
    .footer {
      background: #f4f6f9;
      text-align: center;
      padding: 20px;
      font-size: 0.88em;
      color: #888;
      border-top: 1px solid #e0e0e0;
    }
    .footer a { color: #2e86c1; text-decoration: none; }
  </style>
</head>
<body>
  <div class="container">

    <!-- Header -->
    <div class="header">
      <h1>🏠 House Price Prediction</h1>
      <p>A Machine Learning project to predict house prices using real-world data</p>
      <div class="badges">
        <span class="badge">Python</span>
        <span class="badge">Scikit-learn</span>
        <span class="badge">Pandas</span>
        <span class="badge">NumPy</span>
        <span class="badge">Matplotlib</span>
        <span class="badge">Machine Learning</span>
      </div>
    </div>

    <div class="content">

      <!-- About -->
      <div class="section">
        <h2>📌 About the Project</h2>
        <p>This project predicts house prices based on various features like area, number of bedrooms, bathrooms, city, furnishing status, and more. It uses supervised machine learning algorithms trained on a dataset of 2000 real estate records from cities like Delhi, Mumbai, Pune, Kolkata, and Chennai.</p>
      </div>

      <!-- Workflow -->
      <div class="section">
        <h2>⚙️ Project Workflow</h2>
        <div class="steps">
          <div class="step">
            <div class="icon">📂</div>
            <h4>Data Loading</h4>
            <p>Loaded dataset using Pandas</p>
          </div>
          <div class="step">
            <div class="icon">🧹</div>
            <h4>Preprocessing</h4>
            <p>Handled missing values & outliers</p>
          </div>
          <div class="step">
            <div class="icon">🔍</div>
            <h4>EDA</h4>
            <p>Explored patterns & visualized data</p>
          </div>
          <div class="step">
            <div class="icon">⚙️</div>
            <h4>Feature Engineering</h4>
            <p>Encoded & scaled features</p>
          </div>
          <div class="step">
            <div class="icon">🤖</div>
            <h4>Model Training</h4>
            <p>Trained ML algorithms</p>
          </div>
          <div class="step">
            <div class="icon">📊</div>
            <h4>Evaluation</h4>
            <p>Measured model performance</p>
          </div>
        </div>
      </div>

      <!-- Dataset -->
      <div class="section">
        <h2>📁 Dataset</h2>
        <div class="dataset-box">
          <p>📄 File: <span>enhanced_house_price_dataset.csv</span></p>
          <p>📊 Records: <span>2000 rows</span></p>
          <p>🏙️ Cities: <span>Delhi, Mumbai, Pune, Kolkata, Chennai, Hyderabad</span></p>
          <p>🔑 Features: <span>Area, Bedrooms, Bathrooms, Stories, Parking, Age, Furnishing, City, and more</span></p>
        </div>
      </div>

      <!-- Algorithms -->
      <div class="section">
        <h2>🤖 Algorithms Used</h2>
        <ul class="algo-list">
          <li>📈 <strong>Linear Regression</strong> — Baseline regression model</li>
        </ul>
      </div>

      <!-- Tech Stack -->
      <div class="section">
        <h2>🛠️ Tech Stack</h2>
        <div class="tech-grid">
          <span class="tech-tag">Python</span>
          <span class="tech-tag">Pandas</span>
          <span class="tech-tag">NumPy</span>
          <span class="tech-tag">Scikit-learn</span>
          <span class="tech-tag">Matplotlib</span>
          <span class="tech-tag">Google Colab</span>
        </div>
      </div>
   

  </div>
</body>
</html>
