Image Search Abstraction Layer
================================

--------------------------
User stories:
--------------------------

- I can get the image URLs, alt text and page urls for a set of images relating to a given search string.

- I can paginate through the responses by adding a ?offset=2 parameter to the URL.

- I can get a list of the most recently submitted search strings.


--------------------------
Example usage:
--------------------------

https://shorturl-hr.glitch.me/new/https://www.google.com

https://shorturl-hr.glitch.me/new/https://www.freecodecamp.org/challenges/url-shortener-microservice

https://shorturl-hr.glitch.me/new/www.mongodb.com

--------------------------
Example output:
--------------------------

{"original_url":"https://www.google.com", "short_url":"https://shorturl-hr.glitch.me/4bvowV7R"}

{"original_url":"https://www.freecodecamp.org/challenges/url-shortener-microservice", "short_url":"https://shorturl-hr.glitch.me/7IfLww9S"}

{"error":"Wrong url format, pass a valid protocol and site."}

--------------------------
Usage:
--------------------------

https://shorturl-hr.glitch.me/4bvowV7R

Will redirect to:

https://www.google.com

--------------------------

https://shorturl-hr.glitch.me/7IfLww9S

Will redirect to:

https://www.freecodecamp.org/challenges/url-shortener-microservice


--------------------------
Made by [hr](https://github.com/hrego/)