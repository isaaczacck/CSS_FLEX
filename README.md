# Activity 26
# CSS FLEX

# Instruction:
* Apply CSS Flexbox on 5 pages (e.g., product layout, employee cards, student profiles, etc.)

* Name your repository CSS_FLEX

* Add documentation in the README.md file of your repository

* Submit the GitHub repository link

* Deadline: December 5 2024

## Overview
This Activity demonstrates responsive layouts using CSS Flexbox. Each page showcases a different layout type, including product layouts, employee cards, and more. 

## Pages and Layouts
1. **Product Layout**: Displays products in a responsive grid.
2. **Employee Cards**: Shows employee profiles in a card format.
3. **Student Profiles**: Lists student profiles with images.
4. **Gallery**: A flexible, responsive image gallery.
5. **Services Section**: Highlights different services.

## How to Use Flexbox
Each page uses Flexbox for layout. Here are the primary Flexbox properties used:
- `display: flex;` - Defines a flex container.
- `flex-wrap: wrap;` - Allows items to wrap onto new rows.
- `justify-content` - Aligns items horizontally within the container.

To view the project:
1. Clone the repository: `git clone https://github.com/your-username/CSS_FLEX.git`
2. Open `index.html` in your browser.

   

index.html
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Responsive Flexbox Layout</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <!-- Product Layout Section -->
  <section class="section">
    <h2>Product Layout</h2>
    <div class="container">
      <div class="card">
        <img src="download (3).png" alt="Product 1">
        <h3>Product 1</h3>
        <p>White Mustang 5.0</p>
        <button>Buy Now</button>
      </div>
      <div class="card">
        <img src="shining-purple-mustang-ppe8fwehta3i92ux.jpg" alt="Product 2">
        <h3>Product 2</h3>
        <p>Shining purple Mustang 5.0</p>
        <button>Buy Now</button>
      </div>
      <div class="card">
        <img src="blue.jpg" alt="Product 3">
        <h3>Product 3</h3>
        <p>blue Mustang 5.0</p>
        <button>Buy Now</button>
      </div>
    </div>
  </section>

  <!-- Employee Cards Section -->
  <section class="section">
    <h2>Employee Cards</h2>
    <div class="container">
      <div class="card">
        <img src="bear2.jpg" alt="Employee 1">
        <h3>John</h3>
        <p>Position: Developer</p>
      </div>
      <div class="card">
        <img src="bear2.jpg" alt="Employee 2">
        <h3>Isaac</h3>
        <p>Position: Designer</p>
      </div>
      <div class="card">
        <img src="bear2.jpg" alt="Employee 3">
        <h3>Zaack</h3>
        <p>Position: Manager</p>
      </div>
    </div>
  </section>

  <!-- Student Profiles Section -->
  <section class="section">
    <h2>Student Profiles</h2>
    <div class="container">
      <div class="card">
        <img src="GIRL1.jpg" alt="Student 1">
        <h3>Jane Smith</h3>
        <p>Course: Computer Science</p>
      </div>
      <div class="card">
        <img src="BOY.jpg" alt="Student 2">
        <h3>Mike Johnson</h3>
        <p>Course: Business</p>
      </div>
      <div class="card">
        <img src="GIRL2.jpg" alt="Student 3">
        <h3>Sarah Lee</h3>
        <p>Course: Engineering</p>
      </div>
    </div>
  </section>

  <!-- Gallery Section -->
  <section class="section">
    <h2>Gallery</h2>
    <div class="container">
      <div class="card">
        <img src="bear1.jpg" alt="Gallery Image 1">
      </div>
      <div class="card">
        <img src="bearpic.jpg" alt="Gallery Image 2">
      </div>
      <div class="card">
        <img src="bear3.jpg" alt="Gallery Image 3">
      </div>
    </div>
  </section>

  <!-- Services Section -->
  <section class="section">
    <h2>Our Services</h2>
    <div class="container">
      <div class="card">
        <h3>Service 1</h3>
        <img src="Exceptional-Customer-Service.jpg" alt="Gallery Image 2">
      </div>
      <div class="card">
        <h3>Service 2</h3>
        <img src="Exceptional-Customer-Service.jpg" alt="Gallery Image 2">
      </div>
      <div class="card">
        <h3>Service 3</h3>
        <img src="Exceptional-Customer-Service.jpg" alt="Gallery Image 2">
      </div>
    </div>
  </section>
</body>
</html>

```
styles.css

```
* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
  }
  
  body {
    font-family: Arial, sans-serif;
    line-height: 1.6;
    padding: 20px;
    background-color: #f9f9f9;
  }
  
  h2 {
    margin-bottom: 20px;
    font-size: 1.8em;
    text-align: center;
    color: #333;
  }
  
  .section {
    margin-bottom: 40px;
  }
  
  .container {
    display: flex;
    flex-wrap: wrap;
    gap: 16px;
    justify-content: space-between;
  }
  
  .card {
    background-color: #fff;
    padding: 16px;
    border: 1px solid #ddd;
    border-radius: 8px;
    flex: 1 1 calc(100% - 16px);
    max-width: 100%;
    text-align: center;
  }
  
  .card img {
    width: 100%;
    height: auto;
    border-radius: 8px;
  }
  
  .card h3 {
    font-size: 1.2em;
    margin-top: 8px;
  }
  
  .card p {
    font-size: 0.9em;
    margin: 8px 0;
  }
  
  .card button {
    padding: 8px 16px;
    margin-top: 8px;
    background-color: #007bff;
    color: #fff;
    border: none;
    border-radius: 4px;
    cursor: pointer;
  }
  
  .card button:hover {
    background-color: #0056b3;
  }
  
  /* Responsive styles */
  @media (min-width: 600px) {
    .card {
      flex: 1 1 calc(50% - 16px);
    }
  }
  
  @media (min-width: 900px) {
    .card {
      flex: 1 1 calc(33.333% - 16px);
    }
  }
  
```

## OutPut
[Watch the Video](https://youtu.be/dW1fMrY-2w8)
