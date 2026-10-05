# Lab 1 - www

*Sharing is caring*: each lab participant shares their solution for the following exercise.  

1. Name a website that you like and one that you dislike, and explain why: name at least three reasons for each choice. They can be related, for example, to the structure of the website, the design, functionalities or user interface.

*And now let's get going!*  

2. Using the URL parser [https://url-decode.com/tool/url-parser](https://url-decode.com/tool/url-parser), parse the address 
`https://boutique.tintin.com/en/s-1/search/albums-the_crab_with_the_golden_claws?search_query=milou`
to a find a secret code comprising:
- the last character of the protocol 
- the third character of the domain
- the second character of the Tld
- the second to last character from the file name
- the last character of the query attribute.

3. Introduce the secret code in the address below, replacing the `?` character  
  `https://www.tintin.com/en/characters/?#character`  
  and search for the French name of the character in the text of the accessed web page. (hint: case sensitivity – pay attention to the lower/uppercase!)

4. Add the French name at the end of the address `https://www.tintinpedia.fr/wiki/`
and run the following three tests for the URL thus obtained:  

a.  
[https://http.app/?ref=http.dev](https://http.app/?ref=http.dev) to find out if robots are allowed. What kind of robots? 
Read more about web robots here:  [https://www.robotstxt.org/](https://www.robotstxt.org/)  
b.  
[https://tools.keycdn.com/http2-test](https://tools.keycdn.com/http2-test) to find out if the website allows HTTP2.  
Read more about the differences between the HTTP and HTTP2 protocols here: [https://http.dev/2](https://http.dev/2)  
c.  
[https://www.whatsmyip.org/http-compression-test/](https://www.whatsmyip.org/http-compression-test/) to find out if HTTP compression is allowed.  
Read more about HTTP compression here: [https://http.dev/compression](https://http.dev/compression)  

5. For each of the tests above, we consider that we obtain the value 0 if the test fails, and 1 if it is successeful. Use the status code `s` obtained while running the test from exercise 4 subexercise a,  together with the 0/1 results obtained for the subexercises 4 a, b, c, and compute the following number:  
`n = (a+b)*s + s/(a+2b+c) + c`.  
What is the title of the status code corresponding to n?  
Visit the status code library `https://http.cat/n` (don't forget to replace n with its numerical value) and use your web detective skills to identify the character in the image. Bonus points if you find out the name of the cat. 

6. Coming back to the character described on the page you tested for exercise 4. Identify his best friend. Add the name of this best friend at the beginning of the address `mudhalla.net`. What happens if to the obtained address we also add the 'www' prefix? Use the tester 
[https://http.app/?ref=http.dev](https://http.app/?ref=http.dev) to compare the results of the two HTTP requests (with/without 'www').  
Repeat the test for the address from exercise 2. How do you explain the differences in this case? Read more here: [https://en.wikipedia.org/wiki/World_Wide_Web#WWW_prefix](https://en.wikipedia.org/wiki/World_Wide_Web#WWW_prefix)

7. Use the *Network* tool of your browser (firefox: More Tools/Web Developer Tools/Network; chrome: More Tools/Developer Tools/Network) to identify what types of HTTP methods are invoked when accessing the link from exercise 2. 

   What are the differences between the `GET` and `POST` methods? Read more here: 
   [https://www.w3schools.com/tags/ref_httpmethods.asp](https://www.w3schools.com/tags/ref_httpmethods.asp) 
   and here (on the vulnerabilities of HTTP methods): 
   [https://appcheck-ng.com/http-verbs-security-risks#](https://appcheck-ng.com/http-verbs-security-risks#)

8. Use the *Inspector* tool in your browser to identify the font used for the website at exercise 6.   

9. Using the HTML and CSS editors from *Developer Tools*, modify the website to hide the menu, change its title, colours etc.

#### PREMIUM. Bonus exercises

10. Why do we call the homepage a homepage?  
[https://thehistoryoftheweb.com/why-do-we-call-it-a-homepage/](https://thehistoryoftheweb.com/why-do-we-call-it-a-homepage/)  

11. Link in BIO? To what web pages are we allowed to link?  
[https://thehistoryoftheweb.com/the-right-to-link/](https://thehistoryoftheweb.com/the-right-to-link/) 

12. The voyage to Xanadu. What principle from the Xanadu project you think the web world should adhere to?  
[https://screensresearchhypertext.com/Project-Xanadu](https://screensresearchhypertext.com/Project-Xanadu) 

13. Use the *Developer Tools* and the *Inspector* to visualize content behind a paywall (you can try, for example, to recover the text from this article on [Tim Berners-Lee](https://www.newyorker.com/magazine/2025/10/06/tim-berners-lee-invented-the-world-wide-web-now-he-wants-to-save-it), or this one about [medieval proto-robots](https://www.lrb.co.uk/the-paper/v46/n04/james-vincent/its-rolling-furious-eyes). These websites allowing a limited number of article views. Open some articles until you reach the number of article views allowed, then reopen the article on web or the one on automata and try to find all the hidden text). What do you know about user agents and *Googlebot*?
