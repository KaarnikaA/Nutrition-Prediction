<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Project Documentation Template</title>
    <style>
      /* General Styles */
      body {
        font-family: Arial, sans-serif;
        line-height: 1.6;
        margin: 0;
        padding: 0;
        background-color: #f9f9f9;
        color: #333;
      }

      .container {
        max-width: 900px;
        margin: 0 auto;
        padding: 20px;
      }

      h1,
      h2 {
        font-weight: bold;
      }

      h1 {
        font-size: 2rem;
        margin-bottom: 20px;
      }

      h2 {
        font-size: 1.5rem;
        margin-top: 30px;
        margin-bottom: 15px;
      }

      /* Centered Image */
      .top-image {
        text-align: center;
        margin-bottom: 30px;
      }

      .top-image img {
    width: 100%;
    height: 100%;
    object-fit: cover;
      }

      /* Highlight Box for Research Question */
      .highlight-box {
        background-color: #f5f5f5;
        border-left: 4px solid #ff5252;
        padding: 10px 15px;
        margin-bottom: 20px;
      }

      .highlight-box p {
        margin: 0;
        font-weight: bold;
      }

      /* Data Sources and Progress List */
      ul {
        list-style-type: none;
        padding-left: 0;
      }

      ul li {
        margin-bottom: 10px;
        position: relative;
        padding-left: 25px;
      }

      ul li:before {
        content: "@";
        position: absolute;
        left: 0;
        font-weight: bold;
        color: #ff5252;
      }
    </style>
  </head>
  <body>
    <div class="container">
      <!-- Top Centered Image -->
      <div class="top-image">
        <img src="images\cropdef.jpg" alt="Cropdef">
      </div>

      <!-- Project Title -->
      <h1>Revitilizing Paddy yields with Computer Vision</h1>

      <!-- Research Question -->
      <h2>Project Hypothesis / Research Question</h2>
      <div class="highlight-box">
        <p>
          ❓ Can deep learning models, specifically Convolutional Neural
          Networks (CNNs), accurately detect and classify multiple nutrient
          deficiencies in paddy plants through leaf image analysis with greater
          accuracy than human experts?
        </p>
      </div>

      <!-- Significance of the Problem in real world -->
      <h2>Significance of the Problem</h2>
      <p>
        Nutrient deficiencies in crops significantly impact agricultural
        productivity, affecting growth rates, yield, and overall plant health.
        While visual symptoms appear on leaves, their accurate identification
        requires extensive expertise and is particularly challenging in early
        stages. Traditional manual inspection is time-consuming, subjective, and
        often leads to delayed interventions. An automated, accurate detection
        system could revolutionize crop management by enabling early
        intervention and precise nutrient application.
      </p>

      <!-- Data Sources -->
      <h2>Data Sources</h2>
      <ul>
        <li>
          November 1, 2021: Reached out to a local small business association
        </li>
      </ul>

       <!-- Approach -->
        <h2>Approach</h2>
        <!-- Image Preprocessing Section -->
        <h4>Image Preprocessing</h2>
        <ul>
            <li><span class="highlight">Segmentation:</span> Segmentation of input leaf images into 224×224 pixel blocks</li>
            <li><span class="highlight">Standardization:</span> Standardization of image data for consistent analysis</li>
        </ul>

        <!-- Model Architecture Section -->
        <h4>Model Architecture</h2>

        <h5>Base Model:</h3>
        <ul>
            <li>Pre-trained <span class="highlight">ResNet-50</span></li>
        </ul>

        <h5>Additional Layers:</h3>
        <ul>
            <li><span class="highlight">Dense Layer:</span> 1024 neurons with ReLU activation</li>
            <li><span class="highlight">Output Layer:</span> Matches the number of classes</li>
        </ul>

        <ul>
            <li>Implementation of <span class="highlight">softmax activation</span> for final classification</li>
      <!-- Progress and Findings -->
      <h2>Progress & Findings</h2>

        <p><span class="highlight">Achieved:</span> 97.22% accuracy in nutrient deficiency classification</p>
        <p><span class="highlight">Model Loss:</span> Reduced to 0.1448 after training</p>
         <p><span class="highlight">Model Loss:</span> Successfully identified distinctive features for each deficiency type:</p>       <ul>
            <li><span class="highlight">Nitrogen:</span> Lemon-yellowish green coloration</li>
            <li><span class="highlight">Phosphorus:</span> Stunted dark green appearance</li>
            <li><span class="highlight">Potassium:</span> Yellowish brown leaf tips</li>
            <li><span class="highlight">Zinc:</span> Characteristic brown spots</li>
        </ul>
  </body>
</html>
