# 1. Tell me about yourself .


# 2. Why should we hire you instead of others?


# 3. Tell me about a time you failed in a project.


# 4. What are semantic HTML tags? Why do we use them?
"Semantic HTML tags clearly describe the purpose of the content to both the browser and developers. Examples include <header>, <footer>, <main>, <section>, <article>, and <nav>. While they don’t change the visual result directly, they improve accessibility for screen readers, help search engines understand the page structure, and make code more readable."

# 5. Difference between inline, block, and inline-block elements?
"Inline elements (like <span>, <a>, <img>) only take up as much width as their content and don’t start on a new line. Block elements (like <div>, <p>, <h1>–<h6>) take the full width of the container and always start on a new line. Inline-block elements behave like inline elements but allow you to set width and height, which normal inline elements don’t support."

# 6. How does CSS specificity work? Explain with an example.
"CSS specificity determines which style will be applied when multiple rules target the same element. The priority is: Inline styles (highest) > ID selectors > Class/attribute/pseudo-class selectors > Element/pseudo-element selectors (lowest). If two rules have the same specificity, the one written later in the stylesheet takes priority."

Example:
```html
#title { color: red; }   /* ID → higher priority */
.title { color: blue; }  /* Class → lower priority */
h1 { color: green; }     /* Element → lowest priority */

```
Here, #title wins.

# 7. What are media queries? Why are they important in responsive design?
"Media queries are a feature in CSS that allow us to apply different styles depending on conditions such as screen width, height, or device orientation. They are essential for responsive design because they help ensure a website looks good and functions well on desktops, tablets, and mobile devices."

# 8. [Coding] Create a simple responsive card component with:

Image on top,

Title + description,

A “Read More” button.
 ```html
 <style>
    body {
      font-family: Arial, sans-serif;
      display: flex;
      justify-content: center;
      padding: 20px;
      background: #f4f4f4;
    }
    .card {
      max-width: 400px;
      width: 100%;
      background: #fff;
      border-radius: 12px;
      box-shadow: 0 4px 8px rgba(0,0,0,0.1);
      overflow: hidden;
      text-align: center;
    }
    .card img {
      width: 100%;
      height: auto;
      display: block;
    }
    .card h2 {
      margin: 15px 0;
    }
    .card p {
      padding: 0 15px;
      color: #555;
    }
    .card button {
      margin: 15px 0 20px;
      padding: 10px 20px;
      border: none;
      border-radius: 6px;
      background: #007bff;
      color: #fff;
      cursor: pointer;
    }
    .card button:hover {
      background: #0056b3;
    }
  </style>
</head>
<body>
  <div class="card">
    <img src="https://picsum.photos/400/200" alt="Sample Image">
    <h2>Sunset on the Beach</h2>
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer vel elit at dui condimentum tempus.</p>
    <button>Read More</button>
  </div>
</body>
 ```

Centered on page, 100% width on mobile (<600px), max width 400px on desktop.
# 9. [Explain] How would you make a navbar stick to the top of the page while scrolling?
To make navbar stickt at top we have to first create a navbar at top and few demo content for scrolling purpose.To stick it at the top we can use position fixed with top value 0 and left ,right value 0 .Now the navbar is fixed at top while scrolling
``` html
 <style>
  nav {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    background: #333;
    color: white;
    padding: 10px;
  }
  body {
    margin: 0;
    padding-top: 50px; /* to avoid content hiding under navbar */
  }
  p{
    margin: 200px 0px;
  }
</style>
</head>
<body>


<nav>
  <a href="#">Home</a> | <a href="#">About</a> | <a href="#">Contact</a>
</nav>
<p >Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptatem velit iusto in non officia fuga omnis, eveniet reiciendis, quisquam sed libero sequi vitae illum, nam totam doloremque sit! Consequuntur repudiandae quae, quis nesciunt sit laboriosam iure minima maiores voluptatem animi fuga sapiente recusandae dicta. Ratione, iusto, fuga officia ab impedit voluptatum, ipsam amet consequuntur sunt suscipit quaerat expedita perspiciatis quasi qui quibusdam natus. Tenetur, a ratione quisquam unde rerum praesentium voluptates recusandae molestias possimus fuga suscipit deleniti labore similique. Fugit quod vitae, tempore voluptatum nostrum, officia harum alias distinctio perspiciatis commodi quos cumque a aut, sed reprehenderit ratione eligendi hic doloremque eius? Quidem similique ipsa ad odio commodi, totam pariatur! Quis sint perferendis dolor laborum nulla consequuntur illo aperiam praesentium adipisci nobis soluta eum aspernatur, dicta deleniti quasi ducimus nihil veniam error nam assumenda, consectetur atque et voluptates expedita! Illum possimus autem dignissimos aspernatur aliquid. Alias velit eos dignissimos non natus molestias, obcaecati eius inventore, accusamus ipsum maxime blanditiis, assumenda consequuntur dicta iusto error. Magni iste, praesentium suscipit facere dolore repudiandae deleniti atque sequi architecto, officiis reprehenderit est dignissimos, ipsa provident tempora molestias sapiente eligendi minima animi necessitatibus! Distinctio unde facilis provident ipsum. Illo, corrupti doloremque dolores asperiores impedit ducimus.</p>
<p >Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptatem velit iusto in non officia fuga omnis, eveniet reiciendis, quisquam sed libero sequi vitae illum, nam totam doloremque sit! Consequuntur repudiandae quae, quis nesciunt sit laboriosam iure minima maiores voluptatem animi fuga sapiente recusandae dicta. Ratione, iusto, fuga officia ab impedit voluptatum, ipsam amet consequuntur sunt suscipit quaerat expedita perspiciatis quasi qui quibusdam natus. Tenetur, a ratione quisquam unde rerum praesentium voluptates recusandae molestias possimus fuga suscipit deleniti labore similique. Fugit quod vitae, tempore voluptatum nostrum, officia harum alias distinctio perspiciatis commodi quos cumque a aut, sed reprehenderit ratione eligendi hic doloremque eius? Quidem similique ipsa ad odio commodi, totam pariatur! Quis sint perferendis dolor laborum nulla consequuntur illo aperiam praesentium adipisci nobis soluta eum aspernatur, dicta deleniti quasi ducimus nihil veniam error nam assumenda, consectetur atque et voluptates expedita! Illum possimus autem dignissimos aspernatur aliquid. Alias velit eos dignissimos non natus molestias, obcaecati eius inventore, accusamus ipsum maxime blanditiis, assumenda consequuntur dicta iusto error. Magni iste, praesentium suscipit facere dolore repudiandae deleniti atque sequi architecto, officiis reprehenderit est dignissimos, ipsa provident tempora molestias sapiente eligendi minima animi necessitatibus! Distinctio unde facilis provident ipsum. Illo, corrupti doloremque dolores asperiores impedit ducimus.</p>





</body>
```
# 10. (Bonus) Explain the difference between relative, absolute, and fixed positioning in CSS.
relative positioning is relative to it's root where as absolute positioning is relative to it's parent.fixed position will be fixed at a particular place .In relative we can't give top,bottom,left.right value but incase of absolute and fixed we can define that.