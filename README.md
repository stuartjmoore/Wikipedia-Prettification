# Wikipedia Prettification

I love Wikipedia. I must visit it every day to discover something I just heard about (or catch-up on a history lesson that I missed in high school).

But I don’t like the layout.

The design was always kind of ‘eh’ to me, but it really took a turn for the worse when I tried to read an article on my iPad. It was just a bit too clunky. Going from Google’s awesome iPad search layout to an article on Wikipedia was almost day and night.

Luckily, Wikipedia lets you upload your own CSS and JS to customize every page to your heart’s content. I’ve started working on such a design. I’m not great at CSS and JS, so any input is very welcome.

## How to Use

Log into Wikipedia and visit your [Appearance page](http://en.wikipedia.org/wiki/Special:Preferences#mw-prefsection-rendering). Select MySkin and paste in the custom CSS and JS respectively.

I’ve only tested and ran on Chrome, so it very likely will break on other browers.

## Clear Vertical Reading Line, 24px Rythem, Cleaner Typeface

Wikipedia articles are too all over the place. The infobox and images shift the paragraphs too far right and left, forcing your eye back and forth and hurting scannablity. Like a lot of webpages, the line height of paragraphs is far too small and the width is far too long (usually a percentage of the window size). 

## Hanging Table of Contents, Infobox, & Images

In my design, in order to keep a clear reading experience (Wikipedia is an encyclopedia after all), non-text content is kept off to the side and paragraphs are kept to 560px. The table of contents always felt like it broke the article off too much. I understand that the first section is a broad overview, but it can be sectioned off nicer while maintaining a single flow. 

Similar treatment is applied to the infobox and images. Images vary in size too much, kicking the paragraghs around. I’ve kept them all down (or up) to 200px in width. A larger version will pop-up in a lightbox eventually, with the full-size only a link away.

## Fade-out Links Until Hovering Paragraph

Wikipedia is amazing for it’s wealth of information, proven by its cross-linking. The problem is that each page can look like a distraction of black & blue text. I’ve toned the links down to a dark gray, turning bright blue upon hovering of the paragraph and underlined upon hovering the link.

Probably a controversial change, but it’s an idea I’ve been meaning to try for a while now.

## Rearranged Menus

I had no idea that you could find a list of articles that linked to the current one you were reading. It’s right there, how did I miss it? It’s hidden in a mess of links off to the left.

Not only do I ignore those links, but I would collapse the menus by default. Some links are Wikipedia-wide, some are article-wide, some are user-wide. And yet, they’re all sitting there together.

I’ve pushed them around, hoping they’re a little more obvious. I find myself clicking on “Random Article” and “Current Events” much more than before.

I’ve also hidden some of the items under a drop-down menu. The languages menu is always changing in length and very distracting. It’s right next to the paragraphs with non-latin characters standing out (if you’re reading in English like I do).

## Removed “[Edit]” Links

I didn’t like all these [Edit] links. You can still edit the entire page via the edit link up top. There’s probably a better way to edit anyway. Double-click a paragraph to get an inline editor?

## Hyphenation, Hanging Lists, Curley Quotes, & Ligatures

Some simple JS code to make the articles a little prettier. Hyphenation keeps the right edge more linear. Straight quotes don’t exist (they’re for cheap typewriters). Ligatures are kind of douche-y, but they only take a few lines of code to generate.

## To Be Done

- Fix multiple “Main Article” links
- Fix multi-level hanging lists
- Lightbox JS
- Hover inline citation pop-up
- iPad
-- Drop-down table of content
-- Horizontal infobox?
-- ff ligiture doesn’t work
- Combine Tools and Print drop-down
- Get rid of horizontal scrolling on all pages
- Better alert boxes
- Code for non-Chrome browsers