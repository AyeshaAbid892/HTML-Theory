<div align="center"> 

# 🌐 HTML Theoretical Questions
### 📖 A Complete Reference Guide with Code Examples & Visual References 🖼️

![Subject](https://img.shields.io/badge/Subject-HTML_Theory-4f9ef8?style=for-the-badge)
![Questions](https://img.shields.io/badge/Questions-20_Total-10b981?style=for-the-badge)
![Level](https://img.shields.io/badge/Level-Core-f59e0b?style=for-the-badge)
![Repo](https://img.shields.io/badge/Repo-html--theory-7c3aed?style=for-the-badge)

---

> 💡  All answers written in own words · ⚙️ Code examples included · 👁️ Visual References previews shown

</div>

---

## 📋 Table of Contents

| # | Question | # | Question |
|---|----------|---|----------|
| [Q0](#q0-what-is-html-and-html5) | HTML vs HTML5 | [Q10](#q11-html5-semantic-tags) | Image Formats |
| [Q1](#q1-semantic-html-tags) | Semantic HTML Tags | [Q11](#q11-html5-semantic-tags) | HTML5 Semantic Tags |
| [Q2](#q2-div-vs-span) | `<div>` vs `<span>` | [Q12](#q12-script-async-and-defer) | Script, Async & Defer |
| [Q3](#q3-block-level-vs-inline-elements) | Block vs Inline | [Q13](#q13-embedding-audio--video) | Audio & Video Embed |
| [Q4](#q4-doctype-declaration) | DOCTYPE Declaration | [Q14](#q14-relative-vs-absolute-paths) | Relative vs Absolute Paths |
| [Q5](#q5-id-vs-class-attributes) | id vs class | [Q15](#q15-data-attributes) | Data Attributes |
| [Q6](#q6-html-forms--input-types) | Forms & Input Types | [Q16](#q16-viewport-meta-tag) | Viewport Meta Tag |
| [Q7](#q7-meta-tags-in-html) | Meta Tags | [Q17](#q17-seo-with-html) | SEO with HTML |
| [Q8](#q8-the-alt-attribute) | Alt Attribute | [Q18](#q18-accessibility-best-practices) | Accessibility |
| [Q9](#q9-clickable-images) | Clickable Images | [Q19](#q19-strong-vs-b-and-em-vs-i) | `<strong>` vs `<b>` |

---

## 📁 Q/A Repository

<br>


## `Question 0:`
**HTML and HTML5**

> **HTML** `(HyperText Markup Language)` is the foundation of every webpage, it structures content using tags like headings, paragraphs, and links.<br> **HTML5** is just the newer version of HTML. The main differences are:<br> 
<br>1.`Semantic Tags`:<br> Instead of using generic `<div>` tags everywhere, HTML5 introduces proper tags like `<header>`, `<nav>`, and `<footer>` (as shown in the diagram below).<br> 
2.`Multimedia`:<br> We can now use native `<video>` and `<audio>` tags directly, without needing old plugins like Flash.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>My HTML5 Page</title>
</head>
<body>

    <h1>Hello, HTML5!</h1>
    
    <video controls src="video.mp4"></video> 
    <canvas id="draw"></canvas>               

</body>
</html>
```

**`📸 Visual References:`**

<img width="450" height="250" alt="image" src="https://github.com/user-attachments/assets/3d6ab9d4-49ce-48f4-acf2-947a84e26efd" />




## `Question 1:` 

**Semantic HTML Tags**

> **Semantic tags**  are HTML elements that tell both the browser and the developer what kind of content is inside them.<br> Instead of using a meaningless `<div>` tag for everything, we use tags that actually mean something, like `<header>`, `<nav>`, or `<article>`.<br>
**They are important for a few key reasons:**<br>
<br>1.`Better SEO`: Search engines like Google can scan the page much easier and figure out what the main content is.<br>
2.`Accessibility`: Screen readers used by visually impaired people can navigate the website correctly.<br>
3.`Cleaner Code`: It makes the code much easier to read and update for developers because you instantly know what each section does.<br>

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Semantic vs Non-Semantic</title>
</head>
<body>

    <div class="header">
        <h1>My Site</h1>
    </div>
    <div class="nav">
        <a href="#">Home</a> | <a href="#">About</a>
    </div>
    <div class="content">
        <p>Article text goes here...</p>
    </div>

    <header>
        <h1>My Site</h1>
    </header>
    <nav>
        <a href="#">Home</a> | <a href="#">About</a>
    </nav>
    <article>
        <p>Article text goes here...</p>
    </article>

</body>
</html>
```

**`📸 Visual References:`**

<img width="250" height="300" alt="image" src="https://github.com/user-attachments/assets/8b2d940a-0acf-4084-8867-e73100c66f59" />


---

## `Question 2:`
**`<div>` vs `<span>`**

> The main difference between `<div>` and `<span>` is how they display content on the page:<br>
<br>`<div> (Block-level)`: A div takes up the entire width of the page, meaning it always starts on a new line. We use it as a container to group large sections or build layouts.<br>
`<span> (Inline)`: A span only takes up as much space as the content inside it and stays on the same line. We use it to style small pieces of text inside a sentence without breaking the layout.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Div vs Span Example</title>
</head>
<body>

    <div style="background: lightblue;">I am a div block</div>
    <div style="background: lightcoral;">Another div block</div>

    <p>My favorite color is <span style="color: red;">red</span> always.</p>

</body>
</html>
```

**`📸 Visual References:`**

<img width="1800" height="304" alt="image" src="https://github.com/user-attachments/assets/79741af4-228f-4e5c-a30f-ea7ca812bb5f" />



---

## `Question 3:`
**Block-level** vs **Inline Elements**

> In **HTML**, elements are divided into two main display behaviors:<br>
<br>1.`Block-level elements` always start on a brand new line and stretch out to take up the full width available on the screen. Common examples include headings `(<h1> to <h6>)`, paragraphs `(<p>)`, and list items `(<li>)`.<br>
<br>2.`Inline elements` do not start on a new line. They only take up as much space as their actual content requires and sit directly within the flow of the text. Examples include links `(<a>)`, bold text `(<strong>)`, and images `(<img>)`.<br>
**Note**: As a general rule, block-level elements can act as containers for inline elements, but inline elements shouldn't contain block-level elements.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Block vs Inline</title>
</head>
<body>

    <h1>This is a Heading (block)</h1>
    <p>This is a Paragraph (block)</p>

    <p>
        Visit <a href="#">our website</a> and 
        read <strong>important</strong> updates.
    </p>

</body>
</html>
```

**`📸 Visual Refrences:`**

<img width="500" height="300" alt="image" src="https://github.com/user-attachments/assets/ac8b9244-c565-43d3-8760-883d52d152c9" />


---

## `Question 4:`
**DOCTYPE Declaration**

> The `<!DOCTYPE html>` declaration is an instruction to the web browser telling it exactly which version of HTML the page is written in. It is not an actual HTML tag, and it must always be the very first line of code in your file.<br>
**It is important because:**<br>
<br>1. It forces the browser to load the page in "`Standards Mode`", ensuring that elements render correctly and look the same across different modern browsers.<br>
2.Without it, the browser falls back into "`Quirks Mode`", an old compatibility setting that can cause the website's layout to look broken or behave unpredictably.

```html
<!DOCTYPE html>   <!--  Tells browser: "This is HTML5" -->
<html lang="en">
  <head>
    <title>Correct Rendering</title>
  </head>
  <body>
    <p>This renders in standards mode </p>
  </body>
</html>
```

**`📸 Visual References:`**

<img width="450" height="350" alt="image" src="https://github.com/user-attachments/assets/cc51d2a9-c67a-4f8d-95a6-cf9f702e614a" />


---

## `Question 5:`
**id vs class Attributes**

> The main difference is that an `id` is unique to a single element, while a `class` can be reused across multiple elements.<br>
<br>`id Attribute`: Think of this like a passport number. `Only one element` on a webpage can have a specific ID. We use it for unique landmarks that appear only once, like a main navigation bar or a specific container.<br>
<br>`class Attribute`: Think of this like a uniform. `Multiple elements` can wear the same class to share the same styling. Also, a single element can have more than one class separated by spaces (like a card that is also highlighted).

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>ID vs Class Example</title>
</head>
<body>

    <div id="main-header">Site Header</div>

    <div class="card highlight">Card One (Uses two classes)</div>
    <div class="card">Card Two</div>
    <div class="card highlight">Card Three</div>

</body>
</html>
```


**`📸 Visual References:`**

<img width="601" height="200" alt="image" src="https://github.com/user-attachments/assets/a6b03548-5f89-4c3c-b2e7-777869e9c565" />


---

## `Question 6:` 
**HTML Forms & Input Types**

> We create a form in HTML using the `<form>` tag. It acts as a container for capturing user data and uses attributes like action `(where to send data)` and method `(how to send data, like POST or GET)`.<br>
**The most commonly used input types and form elements are:**<br>
<br>1.`text & password`: Used for basic single-line inputs like names, and hidden text fields for passwords.<br>
2.`email & number`: Modern HTML5 inputs that provide automatic validation and bring up specialized keyboards on mobile devices.<br>
3.`date`: Built-in element that automatically opens a calendar picker.<br>
4.`radio & checkbox`: Radio buttons let users pick one option, while checkboxes allow selecting multiple options.<br>
5.`select & textarea`: Used for drop-down selection menus and multi-line message boxes.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>HTML Form Example</title>
</head>
<body>

    <form action="/submit" method="POST">
        <input type="text" placeholder="Your name" />
        <input type="email" placeholder="Your email" />
        <input type="password" placeholder="Password" />
        <input type="number" min="1" max="100" placeholder="Age" />
        <input type="date" />

        <label><input type="checkbox" /> Remember me</label>
        <br>
        <label><input type="radio" name="size" value="sm" /> Small</label>
        <label><input type="radio" name="size" value="lg" /> Large</label>

        <select>
            <option>Option 1</option>
            <option>Option 2</option>
        </select>
        
        <textarea rows="4" placeholder="Message..."></textarea>

        <button type="submit">Submit</button>
    </form>

</body>
</html>
```

**`📸 Visual References:`**

<img width="600" height="300" alt="image" src="https://github.com/user-attachments/assets/145bec9c-b9ab-4996-afe6-9552b6f975f8" />


---

## `Question 7:`
**Meta Tags in HTML**

> Meta tags are elements placed inside the `<head>` section of a webpage. They provide background information **(metadata)** about the page that users cannot see directly, but browsers, search engines, and social media platforms use to understand the site.<br>
**We use them for a few main reasons:**<br>
<br>1.`charset`: Tells the browser how to render text and special characters correctly.<br>
2.`viewport`: Makes the webpage responsive and mobile-friendly so it automatically fits smartphone screens.<br>
3.`description`: The short summary text that appears under your website's link on Google search results.<br>
4.`Social Previews (og:)`: Controls how the webpage looks `(title, description, and image)` when shared on platforms like Facebook or LinkedIn.

```html
<head>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    
    <meta name="description" content="Learn HTML from scratch in 30 days.">
    
    <meta property="og:title" content="HTML Course">
    <meta property="og:image" content="thumbnail.jpg">
    
    <title>Meta Tags Example</title>
</head>
<body>

    <p>Meta tags work quietly behind the scenes inside the head tag.</p>

</body>
</html>
```

**`📸 Visual References:`**

<img width="500" height="300" alt="image" src="https://github.com/user-attachments/assets/520b2d84-4ac2-4f5d-bdb7-e8749442d586" />


---

## `Question 8:`
**The Alt Attribute**

> The `alt (alternative text)` attribute provides a text description of an image.<br> **It acts as a backup for three main reasons:**<br>
<br>1.`Accessibility`: Screen readers read this text aloud to visually impaired users so they understand the content.<br>
2.`Broken Images`: If the image fails to load due to slow internet, the browser displays this text instead of a blank box.<br>
3.`SEO`: Search engines cannot see pictures, so they use alt text to understand what the image represents.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Alt Attribute Example</title>
</head>
<body>

    <img src="sunset.jpg" alt="Orange sunset over mountain peaks at dusk">

    <img src="divider-line.png" alt="">

    <img src="dog.jpg" alt="image">

</body>
</html>
```

**`📸 Visual References:`**

<img width="500" height="300" alt="image" src="https://github.com/user-attachments/assets/c6a183e3-1b37-41b5-864d-0ec719021997" />


---

## `Question 9:`
**Clickable Images**

> To make an image clickable in HTML, we nest (wrap) the `<img>` tag inside an anchor `<a>` tag.<br>
<br>1.The href attribute on the `<a>` tag defines the destination URL where the user will be taken.<br>
2.You can also add `target="_blank"` if you want the link to open up in a separate new tab instead of the current one.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Clickable Image Example</title>
</head>
<body>

    <a href="https://www.cuterabbit.com">
        <img src="images/rabbit-hero.jpg" alt="Cute Rabbit" class="responsive-hero">
    </a>

</body>
</html>
```

**`📸 Visual References:`**

<img width="600" height="150" alt="Screenshot 2026-05-27 at 10 16 31 PM" src="https://github.com/user-attachments/assets/a6a2ef26-9f0e-4275-9220-41c7927f9c2e" />



---

## `Question 10:`
**Image Formats — JPG, PNG, SVG, WebP**

> Choosing the right image format is important for keeping a website fast while maintaining high-quality visuals.<br> **Here is the direct difference:**<br>
<br>1.`JPG (JPEG)`: Best for complex photographs. It `uses compression` to keep file sizes relatively small, but it does not support transparent backgrounds.<br>
2.`PNG`: Best for logos, icons, and graphics that require a clear or` transparent background`. File sizes are usually larger than JPGs.<br>
3.`SVG`: Unlike other formats, this is a `vector format` based on code. It is infinitely scalable, meaning it will never get blurry or pixelated no matter how big you stretch it. Perfect for UI icons.<br>
4.`WebP`: The modern, standard choice for `web photos`. It offers significantly smaller file sizes than both JPG and PNG without losing any visual quality.

```html
<!-- JPG: photographs and complex images -->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Image Formats Example</title>
</head>
<body>

    <img src="photo.jpg" alt="Mountain landscape">

    <img src="logo.png" alt="Company logo with transparent background">

    <img src="icon.svg" alt="Search icon">
    
    <picture>
        <source srcset="photo.webp" type="image/webp">
        <img src="photo.jpg" alt="Fallback landscape photo">
    </picture>

</body>
</html>
```

**`📸 Visual References:`**

<img width="605" height="300" alt="Screenshot 2026-05-27 at 10 21 13 PM" src="https://github.com/user-attachments/assets/069cf825-db56-4586-b8e2-b54f3c2e257b" />


---

## `Question 11:` 
**HTML5 Semantic Tags**

> Semantic tags are HTML elements that clearly describe their meaning to both the browser and the developer. <br>Instead of using generic `<div>` tags everywhere, these tags define the actual structure and layout of a webpage.<br>
**The core tags introduced in HTML5 are:**<br>
<br>1.`<header>`: Represents the top introductory section of a page, usually containing the website logo and main navigation menu.<br>
2.`<nav>`: Specifically used to wrap block links intended for website navigation.<br>
3.`<main>`: Contains the dominant, unique core content of the document.<br>
4.`<section>`: Groups related content together into thematic chapters or chunks.<br>
5.`<article>`: Defines independent, self-contained content (like a blog post or news story) that could stand alone outside the page.<br>
6.`<aside>`: Used for sidebars or content that is indirectly related to the main text around it.<br>
7.`<footer>`: Placed at the bottom of the page, containing copyrights, privacy policies, or quick links.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Short Semantic Example</title>
</head>
<body>

    <header>
        <h1>Website Title</h1>
    </header>

    <section>
        <h2>Blog Section</h2>
        
        <article>
            <h3>Article Title</h3>
            <p>This is the main content of the post.</p>
        </article>
    </section>

    <footer>
        <p>&copy; 2026 My Website</p>
    </footer>

</body>
</html>
```

**`📸 Visual Refrences:`**

<img width="400" height="400" alt="Screenshot 2026-05-27 at 10 27 12 PM" src="https://github.com/user-attachments/assets/b2ac6a43-5001-4475-b25b-f69510ce6d77" />


---

## `Question 12:`
**Script, Async, and Defer**

> These attributes control how and when JavaScript files are loaded relative to the HTML parsing of the webpage:<br>
<br>1.`Normal <script>`: The browser stops parsing HTML completely to download and run the JavaScript file immediately. This can `slow down page` loading.<br>
2.`async`: JavaScript downloads in the background (parallel) and executes the exact moment it is ready. This can `interrupt HTML` parsing and doesn't guarantee the execution order of multiple scripts.<br>
3.`defer`: JavaScript downloads in the background (parallel) but waits until the HTML parsing is 100% finished before executing. This is usually the `best practice` for performance.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Script Loading Example</title>

    <script src="script.js"></script>

    <script src="async-script.js" async></script>

    <script src="defer-script.js" defer></script>
</head>
<body>

    <h1>Script, Async, and Defer Comparison</h1>

</body>
</html>
```

**`📸 Visual References (Timeline):`**


<img width="600" height="200" alt="image" src="https://github.com/user-attachments/assets/44931680-d727-40e8-abd8-154c79a34c8b" />

<br> 

| Attribute | Download | Execution | Blocks HTML? |
|-----------|----------|-----------|--------------|
| (none) | Sequential | Immediate | ✅ Yes |
| `async` | Parallel | As soon as ready | Sometimes |
| `defer` | Parallel | After HTML parsed | ❌ No |

---

##` Question 13:` 
**Embedding Audio & Video**

> HTML5 allows us to embed audio and video files natively using the `<audio>` and `<video>` tags, without needing any old third-party plugins like Flash Player.<br>
**Key aspects of these tags include:**<br>
<br>1.`controls Attribute`: Adds the default `browser buttons` like play, pause, and volume control so users can interact with the media.<br>
2.`<source> Tags`: Used inside the media player to provide multiple file formats `(like MP4/WebM for video, and MP3/OGG for audio)` so the browser can pick the one it supports.<br>
3.`Fallback Text`: Simple text placed `inside the tags` that only displays if a user is using an outdated browser that doesn't support HTML5 media.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Embedding Media Example</title>
</head>
<body>

    <video width="640" height="360" controls autoplay muted loop>
        <source src="movie.mp4" type="video/mp4">
        <source src="movie.webm" type="video/webm">
        <p>Your browser doesn't support video. <a href="movie.mp4">Download it</a></p>
    </video>

    <audio controls>
        <source src="song.mp3" type="audio/mpeg">
        <source src="song.ogg" type="audio/ogg">
        <p>Your browser doesn't support audio.</p>
    </audio>

</body>
</html>
```

**`📸 Visual References:`**

<img width="600" height="200" alt="Screenshot 2026-05-27 at 10 39 11 PM" src="https://github.com/user-attachments/assets/710835fb-f2de-4338-970b-cf8440f88234" />


---

## `Question 14:`
Relative vs Absolute Paths

> The main difference is how the browser looks for the linked file or resource:<br>
<br>1.`Relative Path`: Points to a file based on your current file's location. It is like giving local directions from where you are standing right now `(e.g., "look inside the current folder" )`. We use this for internal project files.<br>
2.`Absolute Path`: Points to the exact, complete `URL or directory path` from the root. It works from anywhere on the internet regardless of where your current HTML file is stored. We use this for linking external websites or assets.<br> **Note**: Use relative paths for your `own project files`; absolute for `external resources.`

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>File Paths Example</title>
    <link rel="stylesheet" href="../css/style.css">
</head>
<body>

    <img src="https://example.com/logo.png" alt="External Logo">
    <a href="https://google.com">Visit Google</a>

    <img src="images/logo.png" alt="Local Logo">

</body>
</html>
```

**`📸 Visual References:`**

<img width="800" height="300" alt="image" src="https://github.com/user-attachments/assets/e4842b04-3e6e-4cf3-a334-562f6a346edc" />


---

## `Question 15:`
**Data Attributes**

> Data attributes allows us store extra, custom information inside regular HTML tags without breaking any layout rules. Any attribute name that starts with `data-` is valid.<br>
**They are mainly used for:**<br>
<br>1.`JavaScript`: To easily pass data from HTML into scripts using element.dataset.<br>
2.`State Management`: Storing specific info like product IDs, filter categories, or prices right on the element.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Data Attributes Example</title>
</head>
<body>

    <img src="book.jpg" alt="Sherlock Holmes" data-author="Arthur Conan" data-pages="329">

    <div data-product-id="PRD-001" data-price="29.99">
        <p>Product Card</p>
    </div>

</body>
</html>
```



**`📸 Visual References:`**

<img width="350" height="300" alt="image" src="https://github.com/user-attachments/assets/f46612cb-f25d-462d-adba-3662e3151fed" />


---

## `Question 16:` 
**Viewport Meta Tag**

> The viewport meta tag tells the browser how to control a webpage's dimensions and scaling on mobile devices. Without it, mobile browsers render the page as if it were on a desktop, making the text tiny and forcing users to zoom in.<br>
**Here is what its main settings do:**<br>
<br>1.`width=device-width`: Sets the width of the page to match the actual screen width of the device being used (phone, tablet, etc.).<br>
2.`initial-scale=1.0`: Sets the initial zoom level when the webpage first loads, preventing browsers from automatically scaling down the content.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Viewport Example</title>
</head>
<body>

    <h1>Responsive Web Page</h1>
    <p>This page scales perfectly on both desktop and mobile devices.</p>

</body>
</html>
```

**`📸 Visual References:`**

<img width="800" height="200" alt="image" src="https://github.com/user-attachments/assets/91be9cb6-51dc-42ce-96c6-9f5d0c6b7520" />


---

## `Question 17:`
**SEO with HTML**

>` SEO (Search Engine Optimization)` through HTML means structuring your code and content so search engines like Google can easily understand and index your webpage.<br>
**We can achieve this by implementing these key practices:**<br>
<br>1.`Descriptive Meta Tags`: Using a unique `<title>` tag and a `<meta name="description">` tag inside the head section to show a clean snippet on search result pages.<br>
2.`Proper Heading Hierarchy`: Using only one `<h1>` tag for the main topic, followed by sequential subheadings `(<h2>, <h3>, etc.)` to create a clear layout.<br>
3.`Image Alt Text`: Adding descriptive `alt attributes` to all images so search engine bots know what the picture represents.<br>
4.`Semantic Links`: Writing descriptive text inside anchor tags `(<a>)` instead of generic phrases like "click here".

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Buy Handmade Leather Bags | CraftBag Store</title>
    <meta name="description" content="Shop handmade leather bags crafted in Italy. Free shipping on orders over $50.">
</head>
<body>

    <h1>Handmade Leather Bags</h1>
    <h2>Our Best Sellers</h2>
    <h3>The Milano Tote</h3>

    <img src="tote.jpg" alt="Brown leather Milano tote bag with gold buckle">

    <a href="/bags/milano">View the Milano Collection</a>

</body>
</html>
```

**`📸 Visual References:`**

<img width="600" height="250" alt="image" src="https://github.com/user-attachments/assets/e82b4d4e-4bda-470f-aecb-758b8addc025" />


---

## `Question 18:`
**Accessibility Best Practices**

> Web accessibility means coding your website in a way that everyone can use it easily, including people who depend on screen readers, keyboard-only navigation, or have visual impairments.<br>
**Here are the most important practices to follow:**<br>
<br>1.`Use Proper Labels`: Always link form inputs with `<label>` tags so screen readers can tell users exactly what they need to type.<br>
2.`Add ARIA Labels`: Use attributes like `aria-label` to give screen readers extra context on custom components, like close buttons or navigation blocks.<br>
3.`Include Skip Links`: Add a hidden `"Skip to main content"` link at the very top so keyboard-only users don't have to tab through long menus every time.<br>
4.`Keep Headings in Order`: Follow a clean hierarchy `(<h1> then <h2>, then <h3>)` so the structure of the page makes sense immediately.<br>
5.`Set the Language`: Always specify the `<html lang="en">` tag at the start so screen readers know what language pronunciation to use.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Accessibility Best Practices</title>
</head>
<body>

    <a href="#main-content">Skip to main content</a>

    <header>
        <h1>Page Title</h1>
        <nav aria-label="Main navigation">
            <a href="/home">Home</a>
        </nav>
    </header>

    <main id="main-content">
        <h2>Section Heading</h2>

        <label for="username">Username:</label>
        <input type="text" id="username" name="username">

        <button aria-label="Close dialog" onclick="closeModal()">X</button>
    </main>

</body>
</html>
```

**`📸 Visual References:`**

<img width="600" height="250" alt="image" src="https://github.com/user-attachments/assets/2e0dd5e1-c3da-4667-adb1-1d4b4fe61cbd" />


---

## `Question 19:` 
**`<strong>` vs `<b>` and `<em>` vs `<i>`**

> Even though these tags look exactly the same on a screen, they have completely different meanings (semantics) for search engines and screen readers:
<br> `<strong>` vs `<b>` (Bold Text):<br>
<br>1.`<strong>`: Means the content is genuinely important or an urgent warning. Screen readers read this out with a louder or serious tone.<br>
2.`<b>`: Just styles the text to look bold for visual design, carrying absolutely no extra meaning or importance.<br>
<br> `<em>` vs `<i>` (Italic Text):<br>
<br>1.`<em>` (Emphasis): Adds verbal stress or emphasis to a word, which can change the actual meaning of the sentence. Screen readers read this with a stressed voice.<br>
2.`<i>`: Simply tilts the text to italics for purely styling purposes, like formatting book titles, technical terms, or thoughts.<br>

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Semantic Text Tags</title>
</head>
<body>

    <p>
        <strong>Warning: Do not delete this file!</strong>
        The <b>Quick Start Guide</b> is on page 3.
    </p>

    <p>
        I said I <em>love</em> cats – not dogs.
        Read <i>The Great Gatsby</i> this summer.
    </p>

</body>
</html>
```

**`📸 Visual References:`**

<img width="750" height="240" alt="image" src="https://github.com/user-attachments/assets/e5a7804c-4111-4e4e-b35e-689844689b81" />


| Tag | Visual | Semantic Meaning | Screen Reader |
|-----|--------|-----------------|---------------|
| `<strong>` | **Bold** | High importance | Extra emphasis |
| `<b>` | **Bold** | None | Normal |
| `<em>` | *Italic* | Stress emphasis | Stressed reading |
| `<i>` | *Italic* | None (titles, terms) | Normal |

---

<div align="center">

## 🎓 Summary

> This README covers all 20 HTML theoretical concepts with code examples and Visual Refrences previews. Each answer explains the *what*, the *why*, and shows *how it looks* in the browser.

---

**Made with ❤️ for the html-theory repository**

![HTML5](https://img.shields.io/badge/Questions_Covered-20%2F20-success?style=for-the-badge)
![Code Examples](https://img.shields.io/badge/Code_Examples-20-blue?style=for-the-badge)
![Visual Outputs](https://img.shields.io/badge/Visual_Outputs-20-orange?style=for-the-badge)

</div>
