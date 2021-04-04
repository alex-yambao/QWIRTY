# QWIRTY
E-Commerce Site Demo
The Goal of this project was to style and launch a functioning e-commerce website. The guidelines for the project are provided below.

And let's start writing our CSS in footer.css:

Working on the footer itself:
We should set display to flex, and have it flex in a row, so that the child sections will align correctly.
Give it a background color of #255, or something slightly darker than your links in the categories above.
Give it a reasonable amount of padding, something like 18px, or 1rem. You want there to be a bit of color above/below the links themselves.
Continue with the Dosis font in the footer, too.
The sections:
Give them a margin-right, but also clear the margin-right on the last-child (or last-of-type). That will give them each some breathing room.
Set their display to flex, and let them flex in a column. This will let us play with the h2 and a tags with ease.
The h2 tag:
Make it white, give it a white border-bottom, too.
To make the border-bottom appear as if its floating, give it both some padding and margin on the bottom. This will push it away from the words in the h2 as well as the anchor tags below it.
Set a smaller font-size, and prepare to set the font-size for the anchor tags a little smaller still.
Have fun with the letter-spacing property. Add a bit of it to spread out the letters in the headings.
The a tags:
Again: white, no text-decoration, and bold.
Give them a margin-bottom, and set a font-size smaller than the h2 tag.
When hovering over the anchor tag, set a border-bottom of 1px solid white, and also change the margin bottom to be 1px less than the one you set above. This will prevent it from taking up more space.
NOTES
Once you've finished this work, you can copy the HTML from footer.html and categories.html into our index.html, and see the two of them together.

Let's start with the .categories nav:
Since the parent of categories is main, and we've set display: flex to main, we can set the flex properties on .categories. Prevent it from growing, prevent it from shrinking, and set the flex basis to 256px.
Also, let's set the display property to flex, and have it act as a column. This will force the anchor tags inside of it to act as block elements, and to align vertically rather than horizontally.
Now style the anchor tags in side of the categories. Make sure to be specific enough with your CSS selector to avoid styling anchor tags around the whole page with the rules we create.
Remove the text-decoration, change the font-family to 'Dosis', and set the text-align to center.
Buttons generally look good with uppercase text, so give the anchor tags a text-transform.
They should have a margin-bottom at least so that each tag is separate from each other.
The background color I used is #44b, but feel free to choose your own. Something dark with a white text color.
Let's use the :hover pseudo-class to darken the anchor tags, and add a little box shadow when the user hovers over the link. box-shadow: 0 2px 5px -2px black; is a reasonable rule that makes it look like the button is hovering over the page a bit.

Starting with .items:
This is the parent container for our .item cards, so let's give it a display of flex, have it flex in a row and let it wrap
Set the font-family that the cards will inherit from to Open Sans
Set align-items to flex-start (try various settings for it to see what it looks like)
Since we want our cards to be the biggest part of our main, and our main flexes, we can set flex-grow to 1 to ensure it fills that space next to our categories.
Now let's style the .item cards:
They should have a flex-basis of something small (you choose the amount), a flex-grow of 1, and a flex-shrink of 0. You can use the combined flex property to achieve all three. Also, give it a margin since we don't want the cards touching entirely. Give them a margin on the right, and on the bottom. Something like 12px.
Give them a display of flex, a flex-direction of column, so that we can easily lay out the inner card content.
Lastly, add some box-shadow to the cards (see previous day) so they look like modern info cards.
Give the .item-name and .fact-line classes some background color, similar to the overall theme you've chosen.
The .item-name has 2 children, a span with the name and an icon:
If you give .item-name a display of flex, you can set justify-content to space-between to push them away from each other. You can also set align-items to center to get them to center against the horizontal axis.
Give it some padding, and set a good font-size and color.
For .add-item, give it a darker background, and bright color. Additionally, set the border-radius so the icon appears to be round.
Do something similar for the .fact-line, and .item-description.
Time for media queries... When the max-width is 768px:
Inside the media query: set the font-sizes of the sub-classes in the .item card to be larger
Give the .item card a flex-basis of 100%
Have the .items flex in a column rather than a row.
NOTES

There's two navs (.main-nav and .sub-nav) in the header: both should flex.
The main should have a dark background, and should set justify-content to space-between.
The main nav has two nav-lists: .short-width and .full-width:
Set .full-width to display: none and .short-width to display: flex
Add a media query: when min-width is over 768px, and switch the display properties of the two classes above. This will show the menu icon when the screen is narrow, and show the menu items when it is wide.
For the .nav-list class:
Set the display to flex, give it a direction of row.
Have the anchor tags inside get some padding, and a border-right
Remove the border-right on the last anchor tag. To do this, you'll have to target the last li, like this: .nav-list li:last-of-type a { /* stuff */ }
Now for the .sub-nav:
The .search-form should grow to full width, and should itself have a display of flex.
Give the input, and button some styling. You can add padding to both, remove the borders, and give the input a border-bottom equal in color to our color scheme.
Have the input flex-grow so that the search box is the largest part of the form.
Lastly, style the .company-name and .credit-offer to match the screen shots as closely as possible.
