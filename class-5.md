# Choosing Images 
Images can be used to set the tone for a site in less time than it takes to read a description. If
you do not have photographs to use on your website, there are companies who sell stock images.
If you have a page that shows several images (such as product photographs or members of a team) then putting them on a simple, consistent background helps them look better as a group.



# Storing Images
As a website grows, keeping images in a separate folder helps you understand how the site is organized. Here you can see an example of the files for a website; all of the images are stored in a folder called images.If you are using a content management system or blogging platform, there are usually tools
built into the admin site that allow you to upload images, and the program will probably
already have a separate folder for image files and any other uploads.


# Adding Images
# <img>
To add an image into the page
you need to use an <-img>
element. This is an empty
element (which means there is
no closing tag). It must carry the
following two attributes:

# src
This tells the browser where
it can find the image file. This
will usually be a relative URL
pointing to an image on your
own site.

# alt
This provides a text description
of the image which describes the
image if you cannot see it.

# title
You can also use the title
attribute with the <-img-> element
to provide additional information
about the image. Most browsers
will display the content of this
attribute in a tootip when the
user hovers over the image.



![add](https://www.codegrepper.com/codeimages/how-to-add-a-link-to-an-image-in-html.png)


# Height & Width of Images
You will also often see an <-img>
element use two other attributes
that specify its size:

# height
This specifies the height of the
image in pixels.

# width
This specifies the width of the
image in pixels.
Images often take longer to
load than the HTML code that
makes up the rest of the page.
It is, therefore, a good idea to
specify the size of the image
so that the browser can render
the rest of the text on the page
while leaving the right amount of
space for the image that is still
loading



![h&w](https://www.wikihow.com/images/thumb/b/be/Set-Image-Width-and-Height-Using-HTML-Step-3-Version-3.jpg/v4-460px-Set-Image-Width-and-Height-Using-HTML-Step-3-Version-3.jpg.webp)


# Where to Place Images in Your Code
Where an image is placed
in the code will affect how it
is displayed. Here are three
examples of image placement
that produce different results:
1. before a paragraph
The paragraph starts on a new
line after the image.
2. inside the start of a
paragraph
The first row of text aligns with
the bottom of the image.
3. in the middle of a
paragraph
The image is placed between the
words of the paragraph that it
appears in



# Three Rules for Creating Images
1. Save images in the right format:
Websites mainly use images in
jpeg, gif, or png format. If you
choose the wrong image
format then your image might
not look as sharp as it should
and can make the web page
slower to load


2.Save images at the right size:
You should save the image at
the same width and height it will
appear on the website. If
the image is smaller than the
width or height that you have
specified, the image can be
distorted and stretched. If the
image is larger than the width
and height if you have specified,
the image will take longer to
display on the page.

3. Use the correct resolution:
Computer screens are made up
of dots known as pixels. Images
used on the web are also made
up of tiny dots. Resolution refers
to the number of dots per inch,
and most computer screens only
show web pages at 72 pixels
per inch. So saving images at
a higher resolution results in
images that are larger than
necessary and take longer to
download


# color
## Foreground Color
The color property allows you
to specify the color of text inside
an element. You can specify any
color in CSS in one of three ways:
rgb values
These express colors in terms
of how much red, green and
blue are used to make it up. For
example: rgb(100,100,90)
 hex codes
These are six-digit codes that
represent the amount of red,
green and blue in a color,
preceded by a pound or hash #
sign. For example: #ee3e80
color names
There are 147 predefined color
names that are recognized
by browsers. For example:
DarkCyan
We look at these three different
ways of specifying colors on the
next double-page spread

# Background Color
CSS treats each HTML element
as if it appears in a box, and the
background-color property
sets the color of the background
for that box.
You can specify your choice of
background color in the same
three ways you can specify
foreground colors: RGB values,
hex codes, and color names
(covered on the next page).
If you do not specify a
background color, then the
background is transparent.
By default, most browser
windows have a white
background, but browser users
can set a background color for
their windows, so if you want
to be sure that the background
is white you can use the
background-color property on
the <-body> element.


![color](https://s3-ap-southeast-1.amazonaws.com/djamblog/article-040320062407.png)

# Contrast
### Low Contrast
Text is harder to read when
there is low contrast between
background and foreground
colors.
A lack of contrast is particularly
a problem for those with
visual impairments and color
blindness

### High Contrast
Text is easier to read when
there is higher contrast between
background and foreground
colors.
If you want people to read a lot
of text on your page, however,
then too much contrast can
make it harder to read, too.

### Medium Contrast
For long spans of text, reducing
the contrast a little bit improves
readability.
You can reduce contrast by
using dark gray text on a white
background or an off-white text
on a dark background




# CSS3: Opacity
CSS3 introduces the opacity
property which allows you to
specify the opacity of an element
and any of its child elements.
The value is a number between
0.0 and 1.0 (so a value of 0.5
is 50% opacity and 0.15 is 15%
opacity).
The CSS3 rgba property allows
you to specify a color, just like
you would with an RGB value,
but adds a fourth value to
indicate opacity. This value is
known as an alpha value and is
a number between 0.0 and 1.0
(so a value of 0.5 is 50% opacity
and 0.15 is 15% opacity). The
rgba value will only affect the
element on which it is applied
(not child elements).
Because some browsers will
not recognize RGBA colors, you
can offer a fallback so that they
display a solid color. If there are
two rules that apply to the same
element, the latter of the two
will take priority. To create the
fallback, you can specify a color
as a hex code, color name or
RGB value, followed by the rule
that specifies an RGBA value. If
the browser understands RGBA
colors it will use that rule. If it
doesn't, it will use the RGB value.




![](https://static.javatpoint.com/less/images/less-contrast-function3.png)




# CSS3: HSL & H
The hsl color property has
been introduced in CSS3 as an
alternative way to specify colors.
The value of the property starts
with the letters hsl, followed
by individual values inside
parentheses for:
## hue
This is expressed as an angle
(between 0 and 360 degrees).

## saturation
This is expressed as a
percentage.

## lightness
This is expressed as a
percentage with 0% being white,
50% being normal, and 100%
being black.
The hsla color property allows
you to specify color properties
using hue, saturation, and
lightness as above, and adds a
fourth value which represents
transparency (just like the rgba
property). The a stands for:

## alpha
This is expressed as a
number between 0 and 1.0.
For example, 0.5 represents
50% transparency, and 0.75
represents 75% transparency




![](https://miro.medium.com/max/964/1*B2d44wTBqfygLEZ8ZTJXzg.png)





# text
### Techniques That Offer a Wider Choice of Typefaces
There are several ways to use fonts other than those listed on the
previous page. However, typefaces are subject to copyright, so the
techniques you can choose from are limited by their respective licenses

#### font-family
The user's computer needs the
typeface installed. CSS is used to
specify the typeface.

#### font-face
CSS specifies where a font can
be downloaded from if it is not
installed on the computer.


#### Service-based Font-Face
Commercial services give users
access to a wider range of fonts
using @font-face


![](https://i0.wp.com/css-tricks.com/wp-content/uploads/2019/02/faux-true.jpg?ssl=1)




# Specifying Typefaces
## font-family
The font-family property
allows you to specify the
typeface that should be used for
any text inside the element(s) to
which a CSS rule applies.
The value of this property is the
name of the typeface you want
to use.
The people who are visiting
your site need the typeface you
have specified installed on their
computer in order for it to be
displayed. 





# font-size
The font-size property enables
you to specify a size for the
font. There are several ways to
specify the size of a font. The
most common are:
pixels
Pixels are commonly used
because they allow web
designers very precise control
over how much space their text
takes up. The number of pixels is
followed by the letters px.
percentages
The default size of text in
browsers is 16px. So a size of
75% would be the equivalent of
12px, and 200% would be 32px.



![font family](https://www.tutorialbrain.com/wp-content/uploads/2019/02/Font-in-HTML.jpg)



# Bold font-weight
The font-weight property
allows you to create bold text.
There are two values that this
property commonly takes:
normal
This causes text to appear at a
normal weight.
bold
This causes text to appear bold.
In this example, you can see
that the element whose class
attribute has a value of credits
has been bolded.


for more detials please join this link!

[The duckett html book](https://wtf.tw/ref/duckett.pdf)





