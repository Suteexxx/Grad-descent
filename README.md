
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Gradient Descent README</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: linear-gradient(120deg, #1e3c72, #2a5298);
      color: #fff;
      margin: 0;
      padding: 0;
    }
    .container {
      max-width: 900px;
      margin: 40px auto;
      padding: 20px;
      background: rgba(0, 0, 0, 0.6);
      border-radius: 10px;
      box-shadow: 0 0 20px rgba(0,0,0,0.5);
    }
    h1, h2, h3 {
      color: #00d4ff;
    }
    code {
      background: #111;
      padding: 4px 8px;
      border-radius: 5px;
      color: #00ffcc;
    }
    pre {
      background: #111;
      padding: 15px;
      border-radius: 10px;
      overflow-x: auto;
    }
    ul {
      line-height: 1.8;
    }
    .badge {
      display: inline-block;
      padding: 5px 10px;
      margin: 5px;
      border-radius: 5px;
      background: #00d4ff;
      color: #000;
      font-weight: bold;
    }
  </style>
</head>
<body>

<div class="container">
  <h1>🚀 Gradient Descent</h1>
  
  <p>
    Gradient Descent is an optimization algorithm used to minimize a function by iteratively moving in the direction of the steepest descent (negative gradient).
  </p>

  <h2>📌 Types of Gradient Descent</h2>
  <ul>
    <li><b>Batch Gradient Descent</b> – Uses the entire dataset</li>
    <li><b>Stochastic Gradient Descent (SGD)</b> – Uses one data point at a time</li>
    <li><b>Mini-Batch Gradient Descent</b> – Uses small batches</li>
  </ul>

  <h2>📐 Formula</h2>
  <p><code>θ = θ - α * ∇J(θ)</code></p>
  <ul>
    <li><b>θ</b> → Parameters</li>
    <li><b>α</b> → Learning rate</li>
    <li><b>∇J(θ)</b> → Gradient of cost function</li>
  </ul>

  <h2>⚙️ Algorithm Steps</h2>
  <ol>
    <li>Initialize parameters randomly</li>
    <li>Compute gradient of cost function</li>
    <li>Update parameters</li>
    <li>Repeat until convergence</li>
  </ol>

  <h2>💻 Example (Python)</h2>
  <pre>
<code>
import numpy as np

# Sample data
X = np.array([1, 2, 3, 4])
Y = np.array([2, 4, 6, 8])

# Initialize parameters
m = 0
c = 0
lr = 0.01
epochs = 1000

n = len(X)

for _ in range(epochs):
    Y_pred = m * X + c
    
    dm = (-2/n) * sum(X * (Y - Y_pred))
    dc = (-2/n) * sum(Y - Y_pred)
    
    m = m - lr * dm
    c = c - lr * dc

print("Slope:", m, "Intercept:", c)
</code>
  </pre>

  <h2>📊 Applications</h2>
  <ul>
    <li>Linear Regression</li>
    <li>Logistic Regression</li>
    <li>Neural Networks</li>
    <li>Deep Learning Models</li>
  </ul>

  <h2>🏷️ Tech Stack</h2>
  <div>
    <span class="badge">Python</span>
    <span class="badge">NumPy</span>
    <span class="badge">Machine Learning</span>
  </div>

  <h2>📌 Convergence Tips</h2>
  <ul>
    <li>Choose appropriate learning rate</li>
    <li>Normalize data</li>
    <li>Avoid local minima</li>
  </ul>

  <h3>✨ Author</h3>
  <p>Made with ❤️ for learning Machine Learning</p>

</div>

</body>
</html>
