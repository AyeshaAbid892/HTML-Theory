<div align="center">

# 🌐 HTML Theoretical Questions
### A Complete Reference Guide with Code Examples & Visual Outputs

![Subject](https://img.shields.io/badge/Subject-HTML_Theory-4f9ef8?style=for-the-badge)
![Questions](https://img.shields.io/badge/Questions-20_Total-10b981?style=for-the-badge)
![Level](https://img.shields.io/badge/Level-Beginner-f59e0b?style=for-the-badge)
![Repo](https://img.shields.io/badge/Repo-html--theory-7c3aed?style=for-the-badge)

---

> 📘 **All answers written in own words** · Code examples included · Visual output previews shown

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

## Question 0:
What is HTML and HTML5?

> **HTML** (HyperText Markup Language) is the foundation of every webpage — it structures content using tags like headings, paragraphs, and links.<br> **HTML5** is the modern version that adds powerful new features like native audio/video support, semantic elements, canvas drawing, local storage, and much better mobile support — all without needing plugins like Flash.

```html
<!-- Basic HTML5 Document Structure -->
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <title>My HTML5 Page</title>
  </head>
  <body>
    <h1>Hello, HTML5!</h1>
    <video controls src="video.mp4"></video>   <!-- New in HTML5 -->
    <canvas id="draw"></canvas>                <!-- New in HTML5 -->
  </body>
</html>
```

**📸 Output Preview:**

<img width="450" height="250" alt="image" src="https://github.com/user-attachments/assets/3d6ab9d4-49ce-48f4-acf2-947a84e26efd" />




## Q1: Semantic HTML Tags

> **Semantic tags** are HTML elements whose name clearly describes their purpose — for example `<nav>` means navigation, `<article>` means an article. They matter because they help search engines understand page content better (SEO), make websites accessible to screen readers, and make code easier for developers to read and maintain.

```html
<!-- Without Semantics (Bad) -->
<div class="header">My Site</div>
<div class="nav">Home | About</div>
<div class="content">Article text...</div>

<!-- With Semantics (Good) -->
<header>My Site</header>
<nav>Home | About</nav>
<article>Article text...</article>
```

**📸 Output Preview:**

<img width="250" height="300" alt="image" src="https://github.com/user-attachments/assets/8b2d940a-0acf-4084-8867-e73100c66f59" />


---

## Q2: `<div>` vs `<span>`

> `<div>` is a **block-level** container — it takes up the full width of the page and starts on a new line. <br>`<span>` is an **inline** container — it only takes up as much space as its content and stays on the same line. <br> Use `<div>` for sections/layouts, <br> use `<span>` for styling small pieces of text within a sentence.

```html
<!-- div takes full width, breaks line -->
<div style="background: lightblue;">I am a div block</div>
<div style="background: lightcoral;">Another div block</div>

<!-- span stays inline within text -->
<p>My favorite color is <span style="color: red;">red</span> always.</p>
```

**📸 Output Preview:**

<img width="1800" height="304" alt="image" src="https://github.com/user-attachments/assets/79741af4-228f-4e5c-a30f-ea7ca812bb5f" />



---

## Q3: Block-level vs Inline Elements

> **Block-level elements** always start on a new line and stretch across the full available width — examples include `<div>`, `<p>`, `<h1>`, `<ul>`. <br> **Inline elements** sit within the text flow and only occupy as much space as needed — examples include `<span>`, `<a>`, `<strong>`, `<img>`.<br> Block elements can contain inline elements, but not usually the other way around.

```html
<!-- Block Elements -->
<h1>This is a Heading (block)</h1>
<p>This is a Paragraph (block)</p>

<!-- Inline Elements -->
<p>
  Visit <a href="#">our website</a> and 
  read <strong>important</strong> updates.
</p>
```

**📸 Output Preview:**

<img width="500" height="300" alt="image" src="https://github.com/user-attachments/assets/ac8b9244-c565-43d3-8760-883d52d152c9" />


---

## Q4: DOCTYPE Declaration

> The `<!DOCTYPE html>` declaration tells the web browser which version of HTML the page is written in. Without it, browsers enter "quirks mode" — an old compatibility mode that renders pages inconsistently across browsers. It's not an HTML tag; it's an instruction to the browser. Always place it as the very first line of every HTML file.

```html
<!DOCTYPE html>   <!-- ✅ Tells browser: "This is HTML5" -->
<html lang="en">
  <head>
    <title>Correct Rendering</title>
  </head>
  <body>
    <p>This renders in standards mode ✅</p>
  </body>
</html>
```

**📸 Output Preview:**

<img width="450" height="350" alt="image" src="https://github.com/user-attachments/assets/cc51d2a9-c67a-4f8d-95a6-cf9f702e614a" />


---

## Q5: id vs class Attributes

> The `id` attribute is a **unique identifier** — only ONE element on a page can have a specific id. <br>The `class` attribute can be **shared across multiple elements** and one element can have multiple classes. <br> Use `id` for unique landmarks (like a main header). <br> and `class` for reusable styles (like card components or buttons).

```html
<!-- id: unique, used once per page -->
<div id="main-header">Site Header</div>

<!-- class: reusable, many elements can share it -->
<div class="card highlight">Card One</div>
<div class="card">Card Two</div>
<div class="card highlight">Card Three</div>
```


**📸 Output Preview:**

<img width="601" height="200" alt="image" src="https://github.com/user-attachments/assets/a6b03548-5f89-4c3c-b2e7-777869e9c565" />


---

## Q6: HTML Forms & Input Types

> An HTML form collects user data and sends it to a server for processing. <br> The `<form>` tag wraps all inputs, and the `action` attribute defines where data is sent.<br>  HTML5 introduced many new input types like `email`, `date`, `range`, `color`, and `number` that provide built-in validation and mobile-friendly keyboards automatically.

```html
<form action="/submit" method="POST">
  <!-- Common Input Types -->
  <input type="text"     placeholder="Your name" />
  <input type="email"    placeholder="Your email" />
  <input type="password" placeholder="Password" />
  <input type="number"   min="1" max="100" />
  <input type="date"     />
  <input type="checkbox" /> Remember me
  <input type="radio"    name="size" value="sm" /> Small
  <input type="radio"    name="size" value="lg" /> Large
  <select>
    <option>Option 1</option>
    <option>Option 2</option>
  </select>
  <textarea rows="4" placeholder="Message..."></textarea>
  <button type="submit">Submit</button>
</form>
```

**📸 Output Preview:**

<img width="600" height="300" alt="image" src="https://github.com/user-attachments/assets/145bec9c-b9ab-4996-afe6-9552b6f975f8" />


---

## Q7: Meta Tags in HTML

> Meta tags live inside `<head>` and provide **metadata** — information about the page that isn't displayed to users but is read by browsers, search engines, and social media platforms. They control things like character encoding, page description for Google, how the page appears when shared on Twitter/Facebook, and how the page scales on mobile devices.

```html
<head>
  <!-- Character encoding - always include this -->
  <meta charset="UTF-8" />

  <!-- Responsive scaling for mobile devices -->
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />

  <!-- Description shown in Google search results -->
  <meta name="description" content="Learn HTML from scratch in 30 days." />

  <!-- Keywords for search engines (less important now) -->
  <meta name="keywords" content="HTML, CSS, web development" />

  <!-- Open Graph for Facebook/LinkedIn sharing -->
  <meta property="og:title" content="HTML Course" />
  <meta property="og:image" content="thumbnail.jpg" />
</head>
```

**📸 Output Preview:**

<img width="500" height="300" alt="image" src="https://github.com/user-attachments/assets/520b2d84-4ac2-4f5d-bdb7-e8749442d586" />


---

## Q8: The Alt Attribute

> The `alt` attribute on `<img>` tags provides **alternative text** that appears when an image fails to load, and more importantly, is read aloud by screen readers for visually impaired users.<br>  It also helps search engines understand what the image contains. Always write descriptive alt text — not just "image" or "photo". Leave it empty (`alt=""`) only for purely decorative images.

```html
<!-- ✅ Good alt text - descriptive and meaningful -->
<img src="sunset.jpg" alt="Orange sunset over mountain peaks at dusk" />

<!-- ✅ Decorative image - empty alt tells screen reader to skip it -->
<img src="divider-line.png" alt="" />

<!-- ❌ Bad alt text - not helpful at all -->
<img src="dog.jpg" alt="image" />
<img src="dog.jpg" />  <!-- Missing alt entirely! -->
```

**📸 Output Preview:**

<img width="500" height="300" alt="image" src="https://github.com/user-attachments/assets/c6a183e3-1b37-41b5-864d-0ec719021997" />


---

## Q9: Clickable Images

> To make an image clickable in HTML, simply wrap it in an anchor `<a>` tag.<br>  The `href` attribute on the `<a>` tag defines where clicking the image will navigate the user.<br>  You can also add `target="_blank"` to open the link in a new tab. <br> This technique is commonly used for logo images that link back to the homepage.

```html
<!-- Basic clickable image -->
<a href="https://example.com">
  <img src="logo.png" alt="Go to Example website" />
</a>

<!-- Opens in new tab -->
<a href="https://example.com" target="_blank" rel="noopener noreferrer">
  <img src="banner.jpg" alt="Special Offer Banner" width="300" />
</a>
```

**📸 Output Preview:**

<img width="600" height="150" alt="Screenshot 2026-05-27 at 10 16 31 PM" src="https://github.com/user-attachments/assets/a6a2ef26-9f0e-4275-9220-41c7927f9c2e" />



---

## Q10: Image Formats — JPG, PNG, SVG, WebP

> Choosing the right image format affects file size, quality, and how the image behaves. <br> **JPG** is best for photos (lossy compression, small file size). <br>**PNG** supports transparent backgrounds and is best for logos/icons.<br> **SVG** is a vector format that scales to any size without losing quality. <br>**WebP** is a modern format that's smaller than both JPG and PNG while maintaining quality.

```html
<!-- JPG: photographs and complex images -->
<img src="photo.jpg" alt="Mountain landscape" />

<!-- PNG: logos or images needing transparency -->
<img src="logo.png" alt="Company logo with transparent background" />

<!-- SVG: icons and illustrations (infinitely scalable) -->
<img src="icon.svg" alt="Search icon" />
<!-- OR inline SVG -->
<svg width="24" height="24" viewBox="0 0 24 24">
  <circle cx="12" cy="12" r="10" fill="blue" />
</svg>

<!-- WebP: best modern option for photos on web -->
<picture>
  <source srcset="photo.webp" type="image/webp" />
  <img src="photo.jpg" alt="Fallback for older browsers" />
</picture>
```

**📸 Output Preview:**

<img width="605" height="300" alt="Screenshot 2026-05-27 at 10 21 13 PM" src="https://github.com/user-attachments/assets/069cf825-db56-4586-b8e2-b54f3c2e257b" />


---

## Q11: HTML5 Semantic Tags

> HTML5 introduced dedicated semantic tags to replace generic `<div>` containers with meaningful structure.<br> `<header>` contains the page title and navigation. <br>`<footer>` holds copyright and links.<br> `<section>` groups related content. <br>`<article>` represents independent, self-contained content like a blog post that could stand alone on any page.

```html
<body>
  <header>
    <h1>My Blog</h1>
    <nav>
      <a href="/home">Home</a>
      <a href="/about">About</a>
    </nav>
  </header>

  <main>
    <section>
      <h2>Latest Posts</h2>
      <article>
        <h3>Post Title</h3>
        <p>Post content goes here...</p>
      </article>
    </section>

    <aside>
      <h3>Related Links</h3>
    </aside>
  </main>

  <footer>
    <p>&copy; 2024 My Blog. All rights reserved.</p>
  </footer>
</body>
```

**📸 Output Preview:**

<img width="400" height="400" alt="Screenshot 2026-05-27 at 10 27 12 PM" src="https://github.com/user-attachments/assets/b2ac6a43-5001-4475-b25b-f69510ce6d77" />


---

## Q12: Script, Async, and Defer

> These three approaches control **when and how JavaScript files are loaded** relative to HTML parsing.<br> Normal `<script>` blocks HTML parsing until the JS downloads and runs.<br> `async` downloads JS in parallel but runs it immediately when ready (can interrupt parsing). <br>`defer` downloads JS in parallel but waits until HTML is fully parsed before running — this is usually the best choice.

```html
<!-- NORMAL: Blocks HTML parsing ❌ (slow) -->
<script src="app.js"></script>

<!-- ASYNC: Downloads parallel, runs immediately (order not guaranteed) -->
<script async src="analytics.js"></script>

<!-- DEFER: Downloads parallel, runs after HTML parsed ✅ (best) -->
<script defer src="main.js"></script>
```

**📸 Output Preview (Timeline):**


<img width="600" height="200" alt="image" src="https://github.com/user-attachments/assets/44931680-d727-40e8-abd8-154c79a34c8b" />

<br> 

| Attribute | Download | Execution | Blocks HTML? |
|-----------|----------|-----------|--------------|
| (none) | Sequential | Immediate | ✅ Yes |
| `async` | Parallel | As soon as ready | Sometimes |
| `defer` | Parallel | After HTML parsed | ❌ No |

---

## Q13: Embedding Audio & Video

> HTML5 made it possible to embed audio and video natively without any third-party plugins. <br> The `<video>` tag embeds video with playback controls, and <br> `<audio>` does the same for sound. Both support multiple source formats so browsers can pick whichever format they support.<br>  The `controls` attribute adds the built-in play/pause/volume interface.

```html
<!-- Video Embed -->
<video width="640" height="360" controls autoplay muted loop>
  <source src="movie.mp4"  type="video/mp4" />
  <source src="movie.webm" type="video/webm" />
  <p>Your browser doesn't support video. <a href="movie.mp4">Download it</a></p>
</video>

<!-- Audio Embed -->
<audio controls>
  <source src="song.mp3" type="audio/mpeg" />
  <source src="song.ogg" type="audio/ogg" />
  <p>Your browser doesn't support audio.</p>
</audio>
```

**📸 Output Preview:**

<img width="600" height="200" alt="Screenshot 2026-05-27 at 10 39 11 PM" src="https://github.com/user-attachments/assets/710835fb-f2de-4338-970b-cf8440f88234" />


---

## Q14: Relative vs Absolute Paths

> A **relative path** points to a file based on the current file's location — it's like giving directions from where you are now ("go up one folder, then into images"). <br> An **absolute path** includes the full URL or full file path from the root — it works from anywhere regardless of where the current file is located.<br>  Use relative paths for your own project files; absolute for external resources.

```html
<!-- ABSOLUTE PATH: Full URL — works from anywhere -->
<img src="https://mysite.com/images/logo.png" alt="Logo" />
<a href="https://google.com">Visit Google</a>

<!-- RELATIVE PATH: Based on current file location -->
<img src="images/logo.png" alt="Logo" />      <!-- same folder's images/ -->
<img src="../images/logo.png" alt="Logo" />   <!-- go up one folder first -->
<img src="./assets/logo.png" alt="Logo" />    <!-- same directory -->

<!-- ROOT-RELATIVE: Starts from domain root -->
<img src="/images/logo.png" alt="Logo" />
```

**📸 Output Preview:**

<img width="800" height="300" alt="image" src="https://github.com/user-attachments/assets/e4842b04-3e6e-4cf3-a334-562f6a346edc" />


---

## Q15: Data Attributes

> Data attributes (`data-*`) let you store **custom information directly on HTML elements** without breaking HTML standards. <br> Any attribute starting with `data-` followed by your chosen name is valid.<br>  They're perfect for storing IDs, config values, or state information that JavaScript needs to access. You read them in JS using `element.dataset.yourname`.

```html
<!-- Storing custom data on HTML elements -->
<button data-user-id="42" data-role="admin" data-color="blue">
  Edit User
</button>

<div data-product-id="PRD-001" 
     data-price="29.99" 
     data-category="electronics">
  Product Card
</div>
```



**📸 Output Preview:**

<img width="350" height="300" alt="image" src="https://github.com/user-attachments/assets/f46612cb-f25d-462d-adba-3662e3151fed" />


---

## Q16: Viewport Meta Tag

> The viewport meta tag controls how a webpage is **displayed on mobile devices**. Without it, mobile browsers pretend the screen is desktop-width (usually 980px) and scale everything down — making text tiny and requiring users to zoom in. Setting `width=device-width` tells the browser to use the actual screen width, and `initial-scale=1.0` prevents zooming on load.

```html
<!-- Always include in every HTML page for responsive design -->
<meta name="viewport" content="width=device-width, initial-scale=1.0" />

<!-- Advanced options (use carefully): -->
<meta name="viewport" content="width=device-width, 
                                initial-scale=1.0,
                                maximum-scale=1.0,
                                user-scalable=no" />
```

**📸 Output Preview:**

<img width="800" height="200" alt="image" src="https://github.com/user-attachments/assets/91be9cb6-51dc-42ce-96c6-9f5d0c6b7520" />


---

## Q17: SEO with HTML

> SEO (Search Engine Optimization) through HTML means structuring your content in ways that help Google understand it better.<hr> This includes using proper heading hierarchy (`h1` through `h6`), writing descriptive meta descriptions, using semantic tags, adding `alt` text to images, using `<title>` tags effectively, and ensuring clean, fast-loading HTML. Good HTML structure is the foundation of all SEO.

```html
<head>
  <!-- 1. Descriptive, keyword-rich title (50-60 chars) -->
  <title>Buy Handmade Leather Bags | CraftBag Store</title>

  <!-- 2. Meta description (150-160 chars) for search snippets -->
  <meta name="description" content="Shop handmade leather bags crafted in Italy. 
  Free shipping on orders over $50. 100% genuine leather guaranteed." />

  <!-- 3. Canonical URL prevents duplicate content issues -->
  <link rel="canonical" href="https://craftbag.com/leather-bags" />
</head>
<body>
  <!-- 4. One H1 per page — the main topic -->
  <h1>Handmade Leather Bags</h1>

  <!-- 5. H2/H3 for subheadings — clear hierarchy -->
  <h2>Our Best Sellers</h2>
    <h3>The Milano Tote</h3>

  <!-- 6. Descriptive alt text on all images -->
  <img src="tote.jpg" alt="Brown leather Milano tote bag with gold buckle" />

  <!-- 7. Descriptive link text (not "click here") -->
  <a href="/bags/milano">View the Milano Collection</a>
</body>
```

**📸 Output Preview:**

<img width="600" height="250" alt="image" src="https://github.com/user-attachments/assets/e82b4d4e-4bda-470f-aecb-758b8addc025" />


---

## Q18: Accessibility Best Practices

> Web accessibility means building sites that **everyone can use** — <br> including people using screen readers, keyboard-only navigation, or who have visual/motor impairments.<br> Key practices include: always using `alt` text on images, adding `label` elements to form inputs, using proper semantic HTML, ensuring sufficient color contrast, and making everything keyboard-navigable.

```html
<!-- 1. Labels for form inputs (screen readers need this) -->
<label for="username">Username:</label>
<input type="text" id="username" name="username" />

<!-- 2. ARIA roles and labels for custom components -->
<button aria-label="Close dialog" onclick="closeModal()">✕</button>
<nav aria-label="Main navigation">...</nav>

<!-- 3. Skip to content link (keyboard users skip nav) -->
<a href="#main-content" class="skip-link">Skip to main content</a>

<!-- 4. Proper heading hierarchy -->
<h1>Page Title</h1>
  <h2>Section</h2>
    <h3>Subsection</h3>

<!-- 5. Language declaration for screen readers -->
<html lang="en">

<!-- 6. Table with proper accessibility markup -->
<table>
  <caption>Monthly Sales Data</caption>
  <thead>
    <tr><th scope="col">Month</th><th scope="col">Sales</th></tr>
  </thead>
</table>
```

**📸 Output Preview:**

<img width="600" height="250" alt="image" src="https://github.com/user-attachments/assets/2e0dd5e1-c3da-4667-adb1-1d4b4fe61cbd" />


---

## Q19: `<strong>` vs `<b>` and `<em>` vs `<i>`

> These pairs look similar visually but have very different meanings. `<strong>` means the content is **critically important** (screen readers emphasize it). `<b>` just makes text bold for visual styling with no semantic importance. Similarly, `<em>` indicates **stress emphasis** that changes meaning. `<i>` simply italicizes text for stylistic purposes like book titles or technical terms — no extra importance implied.

```html
<!-- STRONG vs B -->
<p>
  <strong>Warning: Do not delete this file!</strong>   <!-- Important! -->
  The <b>Quick Start Guide</b> is on page 3.            <!-- Just styled -->
</p>

<!-- EM vs I -->
<p>
  I said I <em>love</em> cats — not dogs.     <!-- Changes meaning with stress -->
  Read <i>The Great Gatsby</i> this summer.   <!-- Book title — stylistic only -->
</p>
```

**📸 Output Preview:**

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

> This README covers all 20 HTML theoretical concepts with code examples and visual output previews. Each answer explains the *what*, the *why*, and shows *how it looks* in the browser.

---

**Made with ❤️ for the html-theory repository**

![HTML5](https://img.shields.io/badge/Questions_Covered-20%2F20-success?style=for-the-badge)
![Code Examples](https://img.shields.io/badge/Code_Examples-20-blue?style=for-the-badge)
![Visual Outputs](https://img.shields.io/badge/Visual_Outputs-20-orange?style=for-the-badge)

</div>
