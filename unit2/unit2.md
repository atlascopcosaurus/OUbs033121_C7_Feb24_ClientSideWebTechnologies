## Activity 1

```
Write HTML code to display basic information about your institute. Use different tags as described in Table 2.1 to format the structure of your web page.
```

| Tags             | Description                                                       |
| ---------------- | ----------------------------------------------------------------- |
| `<b>`            | It is used to make the text appear bold                           |
| `<i>`            | It is used to make the text look italic                           |
| `<u>`            | It is used to underline the text                                  |
| `<strong>`       | It is used to make important tag look bigger                      |
| `<em>`           | It is used to emphasize the text.                                 |
| `<h1>` to `<h6>` | These tags are used for the headings according to their priority. |
| `<mark>`         | It is used to mark the text                                       |
| `<p>`            | It is used to separate paragraphs.                                |
| `<sub>`          | It is used to make the text subscript.                            |
| `<sup>`          | It is used to make the text superscript.                          |
| `<br>`           | It is used to insert a line break.                                |



Below is an example of HTML code that displays basic information about an educational institute, utilizing the text formatting tags from the Table 2.1 

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Institute</title>
    <style>
        mark { background-color: yellow; }
    </style>
</head>
<body>
    <h1>Welcome to <strong>My Institute</strong></h1>
    <p><em>My Institute</em> is a place of excellence in education since 1950. We are committed to <mark>shaping the future</mark> of our students.</p>

    <h2>Our Programs</h2>
    <p>We offer a range of programs from <sub>undergraduate</sub> to <sup>postgraduate</sup> levels.</p>

    <h2>Contact Us</h2>
    <p>For more information, please contact us:</p>
    <address>
        <strong>Email:</strong> <a href="mailto:info@myinstitute.edu">info@myinstitute.edu</a><br>
        <strong>Phone:</strong> (123) 456-7890<br>
        <strong>Address:</strong> 123 Education Lane, Knowledge City<br>
    </address>

    <h2>Our Values</h2>
    <p><b>Integrity</b>, <i>Innovation</i>, and <u>Excellence</u> are the core values that define us.</p>

    <h2>Testimonials</h2>
    <blockquote>
        <p>"I have had an amazing journey at <strong>My Institute</strong>, with incredible support from the faculty and a rich learning environment."</p>
    </blockquote>
    
    <h2>Alumni Achievements</h2>
    <p>Our alumni have gone on to do great things. They are our pride and they constantly <strong>contribute</strong> back to the society.</p>

    <br>
    <footer>
        <p>&copy; 2024 My Institute. All rights reserved.</p>
    </footer>
</body>
</html>
```

This HTML snippet includes:

- **Heading tags (`<h1>` to `<h2>`):** Used to define headings with `<h1>` being the most important and `<h2>` as a subheading.
- **Bold (`<b>`), Italic (`<i>`), and Underline (`<u>`):** To format text according to their respective styles.
- **Strong (`<strong>`):** To indicate that text is of strong importance, which typically results in bolded text.
- **Emphasize (`<em>`):** To emphasize text, usually italicized.
- **Mark (`<mark>`):** To highlight text.
- **Paragraph (`<p>`):** To define paragraphs.
- **Subscript (`<sub>`) and Superscript (`<sup>`):** For typographical purposes like chemical formulas or mathematical expressions.
- **Line Break (`<br>`):** To insert a single line break.

Remember to replace the placeholder text with actual information about your institute. If you need to serve this HTML file on the web, you would typically save this content in an `.html` file and upload it to a web server.


## Activity 2

```
Apply different text styles discussed in Table 2.2 to the webpage created in Activity 1.
```

To apply the text styles discussed in Table 2.2 to the webpage created in Activity 1, you can add CSS rules within a `<style>` tag in the `<head>` section of the HTML document. Below is an example of how you might apply these styles:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Institute</title>
    <style>
        body {
            font-family: 'Arial', sans-serif; /* Applying font family to the whole page */
            color: #333; /* Default text color */
        }

        h1 {
            background-color: #f0f0f0; /* Background color for h1 */
            text-align: center; /* Center aligning the text */
            font-size: 24px; /* Font size for h1 */
        }

        p {
            color: #555; /* Text color for paragraphs */
            font-size: 16px; /* Font size for paragraphs */
            line-height: 1.6; /* Line height for paragraph spacing */
        }

        .important-text {
            color: #ff0000; /* Making important text red */
            font-weight: bold; /* Adding boldness to important text */
        }

        .highlight {
            background-color: yellow; /* Highlighting text */
        }

        footer {
            text-align: right; /* Right-aligning footer content */
            font-size: 12px; /* Font size for footer */
        }
    </style>
</head>
<body>
    <h1>Welcome to <span class="important-text">My Institute</span></h1>
    <p><em>My Institute</em> is a place of excellence in education since 1950. We are committed to <span class="highlight">shaping the future</span> of our students.</p>

    <!-- Rest of your HTML content goes here -->

    <footer>
        <p>&copy; 2024 My Institute. All rights reserved.</p>
    </footer>
</body>
</html>
```

In this example, I've applied the following styles based on the properties from Table 2.2:

- **background-color:** Applied to the `<h1>` element to change the background color of the text.
- **color:** Applied to the `<p>` element to change the text color, and a special class `.important-text` to change the text color of important words.
- **font-family:** Applied globally to the `body` to change the font writing style of the text on the page.
- **font-size:** Applied to the `<h1>` and `<footer>` to change the text size.
- **text-align:** Applied to the `<h1>` and `<footer>` to align the text accordingly.

Make sure to replace the placeholder text and styles with the actual content and styles that match your institute's branding and preferences.

## Activity 3

```
Write HTML code to create the following lists:

1. Working days
    • Monday
    • Tuesday
    • Wednesday
    • Thursday
    • Friday
2. Off days
    • Saturday
    • Sunday
```

Certainly! Below is the HTML code to create ordered and unordered lists for working days and off days:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Working and Off Days</title>
</head>
<body>
    <h1>Days of the Week</h1>
    
    <h2>1. Working Days</h2>
    <ul>
        <li>Monday</li>
        <li>Tuesday</li>
        <li>Wednesday</li>
        <li>Thursday</li>
        <li>Friday</li>
    </ul>
    
    <h2>2. Off Days</h2>
    <ul>
        <li>Saturday</li>
        <li>Sunday</li>
    </ul>
</body>
</html>
```

This HTML document includes two main parts:

1. An unordered list (`<ul>`) for "Working Days" with list items (`<li>`) for Monday through Friday.
2. Another unordered list for "Off Days" with list items for Saturday and Sunday.

The `<h1>` and `<h2>` tags are used for the main title and subtitles, respectively. If you need the "1." and "2." to be part of the list as per your request, they are included as part of the subtitles rather than the lists themselves because HTML lists automatically only include the list items within the `<ul>` or `<ol>` tags. If you wanted "1." and "2." to be part of an ordered list, you could switch to using the `<ol>` tag instead, but this would number all items sequentially, which doesn't seem to be what you're looking for in this case.


## Activity 4 

```
In the code 2.8 add some more rows and columns in your table and see the output. Also change the border properties to observe the difference in border width.
```

The content of the image you've uploaded seems to refer to HTML code related to the creation of a description list (`<dl>`) rather than a table. However, the instructions mention adding rows and columns to a table and observing the output, as well as changing border properties, which suggests that you might be asking about `<table>` elements instead.

To clarify, `<dl>` is used for a description list, where `<dt>` is used for the term being described, and `<dd>` is for the description of the term. Tables, on the other hand, use `<table>`, `<tr>`, `<th>`, and `<td>` tags.

Assuming you want to create a table with border properties and see the output, here's how you could modify the existing description list to a table with additional rows and columns, and adjust the border width:

```html
<!DOCTYPE html>
<html>
<head>
    <title>Ordered and Unordered items</title>
    <style>
        table {
            border-collapse: collapse;
            width: 100%;
        }
        th, td {
            border: 2px solid black; /* Changing border width */
            padding: 8px;
            text-align: left;
        }
    </style>
</head>
<body>
    <b>Demonstration of Table</b>
    <table>
        <tr>
            <th>Beverage</th>
            <th>Description</th>
        </tr>
        <tr>
            <td>Coffee</td>
            <td>Brown hot drink</td>
        </tr>
        <tr>
            <td>Water</td>
            <td>Transparent cold drink</td>
        </tr>
        <tr>
            <td>Tea</td>
            <td>Milky hot drink</td>
        </tr>
        <!-- Add more rows here -->
        <tr>
            <td>Juice</td>
            <td>Fruit drink</td>
        </tr>
        <tr>
            <td>Soda</td>
            <td>Carbonated water</td>
        </tr>
    </table>
</body>
</html>
```

In this HTML snippet, I have:

- Created a `<table>` element with rows (`<tr>`) and columns (`<th>` for headers and `<td>` for data).
- Applied CSS styles for the table and cells to control the border width (`2px solid black`), which you can change to observe different border widths.
- Added additional rows to the table for "Juice" and "Soda."

To see the output, you would save this HTML code to a `.html` file and open it in a web browser. You can change the `2px` value in the `border` property to a different value, like `1px` or `4px`, to see how the border width changes.




## Activity 5

``` 
Create a web page that contains the links of your favorite travel places.
```

Certainly! Below is an example of a simple HTML web page that contains links to hypothetical favorite travel places. You'll need to replace the URLs with the actual links to your favorite travel destinations:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Favorite Travel Destinations</title>
</head>
<body>
    <h1>My Favorite Travel Places</h1>
    
    <ul>
        <li><a href="https://example.com/paris" target="_blank">Paris, France</a> - The City of Light and Love, home to the Eiffel Tower and Louvre.</li>
        <li><a href="https://example.com/tokyo" target="_blank">Tokyo, Japan</a> - A bustling metropolis blending the ultra-modern with the traditional.</li>
        <li><a href="https://example.com/new-york" target="_blank">New York City, USA</a> - The Big Apple, known for its skyline and Broadway shows.</li>
        <li><a href="https://example.com/machu-picchu" target="_blank">Machu Picchu, Peru</a> - An ancient Incan city set high in the Andes Mountains.</li>
        <li><a href="https://example.com/venice" target="_blank">Venice, Italy</a> - The City of Canals, famous for its waterways and gondolas.</li>
        <li><a href="https://example.com/sydney" target="_blank">Sydney, Australia</a> - Known for its Sydney Opera House and Harbour Bridge.</li>
    </ul>
</body>
</html>
```

To use this HTML:

1. Copy the HTML code above into a text editor.
2. Replace `https://example.com/` with the actual URLs of the travel destinations.
3. Save the file with a `.html` extension, for example, `favorite-places.html`.
4. Open the saved file in a web browser to view the webpage.

The `target="_blank"` attribute in the anchor (`<a>`) tag is used to open the link in a new browser tab or window, which is a common behavior for external links. This ensures that users can easily return to the original list after viewing a destination.



## Activity 6

```
Create a simple web page and add plugins to read different multimedia objects (audio, videos etc.)
```

Creating a simple web page that includes multimedia objects like audio and video can be done by using the HTML5 `<audio>` and `<video>` elements. Here's an example of how to create such a web page:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Multimedia Web Page</title>
</head>
<body>
    <h1>Welcome to My Multimedia Web Page</h1>
    
    <h2>Audio Example</h2>
    <audio controls>
        <source src="path-to-your-audio-file.mp3" type="audio/mpeg">
        Your browser does not support the audio element.
    </audio>
    
    <h2>Video Example</h2>
    <video controls width="250">
        <source src="path-to-your-video-file.mp4" type="video/mp4">
        <source src="path-to-your-video-file.ogg" type="video/ogg">
        Your browser does not support the video tag.
    </video>

    <!-- You can add more multimedia elements here -->

    <footer>
        <p>Thank you for visiting!</p>
    </footer>
</body>
</html>
```

To use this HTML template:

1. Replace `path-to-your-audio-file.mp3` with the actual path to your audio file.
2. Replace `path-to-your-video-file.mp4` and `path-to-your-video-file.ogg` with the actual paths to your video files. It's good practice to provide video in multiple formats for better cross-browser compatibility.
3. Save the HTML code to a file with a `.html` extension, such as `multimedia.html`.
4. Open the file in a web browser to view the web page and test the multimedia playback.

Make sure that the multimedia files are located in the correct path relative to your HTML file or provide an absolute URL to the files. The `controls` attribute is added so that users can play, pause, and control the volume of the audio and video.

Please note that for actual web deployment, you must ensure that you have the rights to use and distribute the multimedia content you are embedding.


## Activity 7

```
Create a web page that can take pizza order from the user. The form may comprise of name and address as text fields, pizza size (small, medium, large) as radio buttons, pizza toppings (cheese, mushrooms, pepperoni) as check boxes and phone number as number field.
```

Below is an example of an HTML web page that includes a form for ordering pizza. The form includes fields for name, address, pizza size, pizza toppings, and phone number:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Pizza Order Form</title>
</head>
<body>
    <h1>Pizza Order Form</h1>

    <form action="/submit-your-order-url" method="post">
        <label for="name">Name:</label><br>
        <input type="text" id="name" name="name" required><br><br>

        <label for="address">Address:</label><br>
        <input type="text" id="address" name="address" required><br><br>

        <label for="phone">Phone Number:</label><br>
        <input type="number" id="phone" name="phone" required><br><br>

        <p>Pizza Size:</p>
        <input type="radio" id="small" name="size" value="small">
        <label for="small">Small</label><br>

        <input type="radio" id="medium" name="size" value="medium" checked>
        <label for="medium">Medium</label><br>

        <input type="radio" id="large" name="size" value="large">
        <label for="large">Large</label><br><br>

        <p>Pizza Toppings:</p>
        <input type="checkbox" id="cheese" name="toppings" value="cheese">
        <label for="cheese">Cheese</label><br>

        <input type="checkbox" id="mushrooms" name="toppings" value="mushrooms">
        <label for="mushrooms">Mushrooms</label><br>

        <input type="checkbox" id="pepperoni" name="toppings" value="pepperoni">
        <label for="pepperoni">Pepperoni</label><br><br>

        <input type="submit" value="Submit Order">
    </form>
</body>
</html>
```

In this form:

- The `action` attribute of the form should be the URL where you want to send the form data to be processed.
- The `method` attribute is set to "post" because you are submitting sensitive user data that should not be visible in the URL.
- Each input field has an associated `<label>` for accessibility reasons. The `for` attribute of the label corresponds to the `id` of the input it is labeling.
- The `required` attribute on the input fields will ensure that the user cannot submit the form without filling out these fields.
- The pizza size is represented by radio buttons, allowing the user to select one option.
- The pizza toppings are represented by checkboxes, allowing the user to select multiple options.
- The "Submit Order" button is used to send the form data to the server for processing.

To see this form in action, you would need to replace `/submit-your-order-url` with the URL of the server-side script that will process the order, and then save the HTML code to a `.html` file. Open this file in a web browser to interact with the form.

## Review Questions
```
Write short answers to the following questions :

1. Describe the basic concept of HTML.
2. Briefly explain the structure of HTML DOM?
3. Which tags are used to bold, italic and underline a piece of text in HTML?
4. Differentiate between ordered and unordered lists.
5. How can you add a space between cell border and the content inside the cell?
6. What are the functions of rowspan and colspan in HTML tables?
7. What is the use of plugin in HTML?
8. Briefly describe different input types available in HTML forms.
```
1. **Basic Concept of HTML:**
   HTML (HyperText Markup Language) is the standard markup language used to create web pages. It provides the structure of a webpage, which includes text, images, links, and other elements, by using a set of elements represented by tags. Browsers interpret HTML files to display formatted content on the web.

2. **Structure of HTML DOM:**
   The HTML DOM (Document Object Model) is a programming interface for HTML documents. It represents the page so that programs can change the document structure, style, and content. The DOM represents the document as a tree of nodes, where each node corresponds to a part of the document (elements, attributes, text, etc.).

3. **Tags for Text Styling in HTML:**
   - **Bold:** `<b>` or `<strong>` (the latter also indicates importance)
   - **Italic:** `<i>` or `<em>` (the latter also conveys emphasis)
   - **Underline:** `<u>` (typically used for stylistic purposes rather than semantic importance)

4. **Difference Between Ordered and Unordered Lists:**
   - **Ordered Lists (`<ol>`):** Display elements in a numbered format, indicating a sequence or ranking.
   - **Unordered Lists (`<ul>`):** Present elements in a bulleted format without any particular order.

5. **Adding Space Between Cell Border and Content:**
   This is achieved by using the `padding` property in CSS. For instance, `padding: 10px;` applied to a `<td>` or `<th>` element would create a 10px space around the content inside the cell.

6. **Functions of Rowspan and Colspan in HTML Tables:**
   - **Rowspan:** Allows a single table cell to span the height of more than one cell or row.
   - **Colspan:** Enables a single table cell to span the width of more than one cell or column.

7. **Use of Plugin in HTML:**
   Historically, plugins in HTML were used to embed external applications that provide certain types of content that the browser might not inherently support, such as Flash or Java applets. However, with the advancement of HTML5, many needs for plugins have been replaced by native HTML, CSS, and JavaScript features.

8. **Different Input Types in HTML Forms:**
   - **Text:** Allows the user to enter a single line of text.
   - **Password:** Similar to text but hides the input.
   - **Radio:** Lets the user select one option from a set.
   - **Checkbox:** Allows the user to select multiple options.
   - **Submit:** Sends form data to a server.
   - **Reset:** Resets the form fields to their default values.
   - **Button:** A clickable button with no default behavior.
   - **File:** Allows the user to select a file to upload.
   - **Hidden:** Stores data that is not visible to the user but can be submitted.
   - **Image:** Defines an image input that can submit form data.
   - **Number:** Lets the user enter a numeric value.
   - **Date, Time, Email, URL:** Specific inputs that allow for the collection of structured data.
   
These input types help ensure that the form data is correctly formatted and can be validated before being sent to a server.



## Coding Exercise

```
1. Create a web page that gives basic information about your hometown. The page should display some interesting facts and figures in a well-designed and attractive way. Also insert some images in your web page.

2. Create a web page about your favorite topic. Insert some interesting YouTube videos in a structured way.

3. Create a basic admission form in HTML which takes basic information like name, father name, postal address, gender (using radio buttons), city and program (using dropdown list), telephone number and email address.
```

Below are the basic HTML templates for the three tasks:

### 1. Web Page about Hometown

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Hometown</title>
</head>
<body>
    <h1>Welcome to My Hometown</h1>
    <p>My hometown is known for its vibrant culture and rich history. It is located in the heart of the country and offers a blend of traditional and modern attractions.</p>
    
    <!-- Insert an image of your hometown -->
    <img src="path-to-your-hometown-image.jpg" alt="Hometown Image" width="500">
    
    <h2>Interesting Facts</h2>
    <ul>
        <li>Founded in the year 1234.</li>
        <li>Known for the annual cultural festival.</li>
        <li>Birthplace of several historical figures.</li>
    </ul>

    <h2>Quick Figures</h2>
    <p>Population: 1.2 million</p>
    <p>Area: 150 square miles</p>
</body>
</html>
```

Remember to replace `path-to-your-hometown-image.jpg` with the actual image path.

### 2. Web Page about Favorite Topic

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Favorite Topic</title>
</head>
<body>
    <h1>Everything about Space Exploration</h1>
    <p>Space exploration is fascinating because it extends human reach beyond Earth. Here are some curated videos about recent space missions and discoveries.</p>

    <!-- Insert YouTube videos -->
    <iframe width="560" height="315" src="https://www.youtube.com/embed/VIDEO_ID" frameborder="0" allowfullscreen></iframe>
    <iframe width="560" height="315" src="https://www.youtube.com/embed/ANOTHER_VIDEO_ID" frameborder="0" allowfullscreen></iframe>

    <!-- Add more videos as needed -->
</body>
</html>
```

Replace `VIDEO_ID` and `ANOTHER_VIDEO_ID` with the actual IDs of the YouTube videos.

### 3. Basic Admission Form

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Admission Form</title>
</head>
<body>
    <h1>Admission Form</h1>
    <form action="submit-form-url" method="post">
        <label for="name">Name:</label><br>
        <input type="text" id="name" name="name" required><br><br>

        <label for="fatherName">Father's Name:</label><br>
        <input type="text" id="fatherName" name="fatherName" required><br><br>

        <label for="address">Postal Address:</label><br>
        <input type="text" id="address" name="address" required><br><br>

        <label>Gender:</label><br>
        <input type="radio" id="male" name="gender" value="male" required>
        <label for="male">Male</label><br>
        <input type="radio" id="female" name="gender" value="female" required>
        <label for="female">Female</label><br><br>

        <label for="city">City:</label><br>
        <input type="text" id="city" name="city" required><br><br>

        <label for="program">Program:</label><br>
        <select id="program" name="program">
            <option value="undergraduate">Undergraduate</option>
            <option value="postgraduate">Postgraduate</option>
            <option value="phd">PhD</option>
        </select><br><br>

        <label for="phone">Telephone Number:</label><br>
        <input type="tel" id="phone" name="phone" required><br><br>

        <label for="email">Email Address:</label><br>
        <input type="email" id="email" name="email" required><br><br>

        <input type="submit" value="Submit">
    </form>
</body>
</html>
```

Replace `submit-form-url` with the actual URL where you want to process the form submission. Ensure you have backend logic to handle the POST request.