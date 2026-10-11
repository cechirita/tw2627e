# Lab 2 - html

*Use the lecture notes to revise the main HTML elements and solve the following exercises.*  

In the *resources* directory you can find screenshots of two web pages: `index-screenshot.png` and `mario-screenshot.png`. Your task is to reproduce the pages in the images using the other available resources (images and text) by following the instructions below. 

## index.html 

1. Decide on the general structure of the file, keeping in mind that the page has three main parts: header, content, and footer. The content is divided in three parts as well: 8-bit games, 8-bit graphics, 8-bit music. Choose the appropriate structuring HTML elements (`header`, `h1`-`h6`, `section`, `article` etc.).

2.  Add the content of the header: title, "8-bit world", and the menu (*hint: use the appropriate navigation HTML element*). 

3. Add the content of the first part, 8-bit games:

- Use an ordered list for the ranking of the most popular games. Add a hyperlink to the `mario.html` page, which you will have to write to solve exercises 6-9.
- Use the `iframe` element to integrate the programming module for NES. 

4. Add the content of the second part, 8-bit graphics:

- Use the HTML `figure` element to include the image `256colour.png`. 
- Use an unordered list to enumerate the main applications of 8-bit graphics. 
- Play with [make8bitart](https://make8bitart.com/) and [8bitworkshop](https://8bitworkshop.com/dithertron) in a burst of 8-bit inspiration. :-)
- Careful when integrating the two youtube videos. What HTML element would be more appropriate? `Video` or `iframe`?

5. Add the content of the last part, 8-bit music. Play with the [Commodore64](https://www.igorski.nl/application/websid/) player to recreate the music of your favourite 8-bit game. :-) 

## mario.html
6.  Decide on the general structure of the file `mario.html`. *Hint: use elements `section` and `article`.*
7. The soundtrack is available [here](https://downloads.khinsider.com/game-soundtracks/album/super-mario-bros/01.%2520Ground%2520Theme.mp3). Save it on your computer and integrate it using the `audio` element.
8. To define the tabel, use the attributes `rowspan` and `colspan` of elements `th` and `td`.
9. Play Super Mario Bros! 

## EXTRA

10. Read [here](https://www.onrec.com/news/news-archive/what-is-8-bit-graphics-and-how-it%E2%80%99s-used-nowadays) more about 8-bit graphics. Is it still used these days? Why?
11. What happens when you reach the 256-th level of Pac-Man? Why couldn't Link gather more than 255 de rupees in Legend of Zelda?  
12. Add more content on the 8-bit world to your HTML pages.

