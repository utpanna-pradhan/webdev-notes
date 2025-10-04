# 1. [Coding] Create a simple responsive card component with:
Centered on page, 100% width on mobile (<600px), max width 400px on desktop.
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
 
# 2. How would you make a navbar stick to the top of the page while scrolling?
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
# 3. Write a function to count the number of vowels in a string.
```html
function countVowels(str) {
  const vowels = ['a', 'e', 'i', 'o', 'u'];
  let count = 0;

  for (let char of str.toLowerCase()) {
    if (vowels.includes(char)) {
      count++;
    }
  }
  return count;
}

console.log(countVowels("Hello Utpanna"));
```
# Q4. Write a function to check if a string is a palindrome. (Don’t use reverse()).
function checkpal(str){
    let tempstr = "";
    for (let i=str.length-1;i>=0;i--){
        tempstr += str[i]
       }
      if(tempstr === str){
           return true;
           
        }
        return false;
   
}
console.log(checkpal("racecar"));

# Q5. Write a function to remove duplicates from an array.
function removeDuplicate(arr){
    return [...new Set(arr)];
}
console.log(removeDuplicate([1,2,34,1,2,3,5]));
# Q6. Write a function to fetch data from an API endpoint (https://jsonplaceholder.typicode.com/posts) and print the titles.
``` HTML
<body>
    <!-- # Q6. Write a function to fetch data from an API endpoint (https://jsonplaceholder.typicode.com/posts) and print the titles. -->
     <div class="card">
        <div class="card">
            
        </div>
     </div>

</body>
<script>
   fetch('https://jsonplaceholder.typicode.com/posts') // Replace with your API endpoint
  .then(response => {
    // Check if the response was successful (e.g., status code 200)
    if (!response.ok) {
      throw new Error(`HTTP error! status: ${response.status}`);
    }
    return response.json(); // Parse the response body as JSON
  })
  .then(data => {
    console.log(data); 
   let container = document.querySelector(".card");

        // Loop through all posts
        data.forEach(post => {
          // Create a new <h1> for each title
          let titleElement = document.createElement("h1");
          titleElement.textContent = post.title;  // use title, not id
          container.appendChild(titleElement);
        });
     
  })
  .catch(error => {
    console.error('Error fetching data:', error); // Handle any errors
  });
   
</script>
```
# 7. Write a function to reverse a string in JavaScript without using reverse().
``` HTML 
function reverseStr(str){
  const revstr="";
  for(let i = str.length-1;i>=0;i--){
    revstr += str[i];
  }
  return revstr;
}
console.log(reverseStr("Hello))
```
