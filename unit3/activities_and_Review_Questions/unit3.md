# Unit 3 : Basics of CSS

## Activity 1

```
Create a simple webpage and display the following information

Brief History of AIOU

The Allama Iqbal Open University was established in May 1974, with the main objectives of providing
educational opportunities to masses and to those who cannot leave their homes and jobs. During all these
years, the university has fulfilled this promise.
Change the font color and size of above text by using Inline CSS method. See the output in your browser
and observe the effects of CSS.
```

Here's how you can create a simple webpage with inline CSS to display the brief history of AIOU:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>AIOU History</title>
</head>
<body>
    <p style="color: blue; font-size: 18px;">
        Brief History of AIOU<br><br>
        The Allama Iqbal Open University was established in May 1974, with the main objectives of providing educational opportunities to masses and to those who cannot leave their homes and jobs. During all these years, the university has fulfilled this promise.
    </p>
</body>
</html>
```

This code snippet uses inline CSS to change the color of the paragraph text to blue and the font size to 18 pixels.


## Activity 2

```
Modify the web page created in activity 1. Change the attributes (font size and color) of the paragraph by using ID selector.
```


To modify the webpage by using an ID selector in CSS, you would first add an `id` attribute to your paragraph, and then write CSS rules in a `<style>` tag within the `<head>` section of the document:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>AIOU History</title>
    <style>
        #aiouHistory {
            color: green; /* Change as desired */
            font-size: 20px; /* Change as desired */
        }
    </style>
</head>
<body>
    <p id="aiouHistory">
        Brief History of AIOU<br><br>
        The Allama Iqbal Open University was established in May 1974, with the main objectives of providing educational opportunities to masses and to those who cannot leave their homes and jobs. During all these years, the university has fulfilled this promise.
    </p>
</body>
</html>
```

In this code snippet, the `id` attribute with the value "aiouHistory" has been added to the `<p>` element, and the `#aiouHistory` selector is used within the `<style>` tag to apply font color and size styles. You can change the color and font size values to observe different effects.



## Activity 3

Code 3.2

```html
<!DOCTYPE html>
<html>
<head>
<title>Background Properties</title>
<style>
body /* Set background properties in body */
{
    background-image: url("schemo.png");
    background-color: white;
    background-repeat: no-repeat;
    background-position: top right;
}
p
{
    font-size: 25px;
}
</style>
</head>
<body>
<p>We give background image and set this image to top right side
<br> of the page with the help of background properties. </p>
</body>
</html>
```

```
Modify the code 3.2 by changing the “background color” of the document to red and “background-repeat” to repeat property.
```


Based on the image content you've provided, here's how you can modify the HTML code to change the "background-color" to red and the "background-repeat" property to "repeat":

```html
<!DOCTYPE html>
<html>
<head>
<title>Background Properties</title>
<style>
body /* Set background properties in body */
{
    background-image: url("schemo.png");
    background-color: red; /* Background color changed to red */
    background-repeat: repeat; /* Background image will now repeat */
    background-position: top right;
}
p
{
    font-size: 25px;
}
</style>
</head>
<body>
<p>We give background image and set this image to top right side
<br> of the page with the help of background properties. </p>
</body>
</html>
```

With these changes, the background image will repeat across the entire body of the web page, and wherever the image is not covering, the background will be red. Remember to replace `"schemo.png"` with the actual path to your background image.


## Activity 4

```
Specify the following properties in the text of above document :

I. Heading should be of 20 points and bold.
II. Paragraph text should be in red color, left justified and indented by 20 points.
```

## Activity 5

```
Create a simple web page with three small paragraphs enclosing each in different types of borders.
```

## Activity 6

```
Create a table with five English words in the first column and their meaning in the second column. Use
table properties to adjust the border, text alignment and font size of the text. Also modify the code by
using “border-collapse” property and see its effect on your table.
```

## Activity 7

```
Create a simple web page with three paragraphs. Enclose each paragraph in different box models by giving
different dimensions such as background-color, border-color and margin properties.
```

## Activity 8

```
Download a scenic image of your choice and change the opacity of image by giving different value and see
the effects.
```

## Activity 9

```
I. Modify code 3.7 and add more links to the vertical navigation bar.

II. Modify code 3.8 and add more links to the horizontal navigation bar.

```

## Activity 10
```
Modify the code 3.9 and change the color, font-size and other properties. Also add some more sub menus
in the dropdown list.
```

## Activity 11

```
Download your favorite images and create image gallery by using CSS. Also adjust the height and width of
images to make your web page look attractive.
```


## Review Questions

```
Write short answers of the following questions :

1. Briefly describe basic concept of CSS.
2. Write different ways to apply style to a web page.
3. What is the difference between attribute and property?
4. What is the difference between class and id selector?
5. How do you add comments in CSS?
6. What is the concept CSS box model and why it is used?
7. Describe the method of creating image gallery in CSS.
8. What is attribute selector and how it is used?

```

## </> Coding Exercise

```
1. Create a web page that gives basic information about your hometown. Use CSS to display
information in a well-designed and attractive way.
2. Create a web page that displays your mark sheet. Use table and text properties to define different
borders and text styles in your web page.
3. Download your favorite pictures from your Facebook account. Create an album of image galleries
using CSS.
```