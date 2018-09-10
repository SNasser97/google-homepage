# the_odin_project - google homepage project
TheOdinProject - HTML+CSS Fundamentals Project

[Nasser Ahmed's Solution (Easy)](https://github.com/SNasser97/google-homepage) - [View in Browser](https://snasser97.github.io/google-homepage/)

Some notes:
I viewed the webpage agan on my laptop since I was using a my desktop to develop this mainly with a ultrawide monitor.
From viewing on the laptop (and on theodinproject site) theres additional space under the footer.

THis is due to the container being set to min-height of 900px, changing the height to 100vh/100% fixes this on viewing on the laptop, however the search section overlaps on the GOOGLE logo.

Using chrome dev tools here is the solution I came up with for when I viewed it on my laptop:

.container {
    width: 100%;
    position: relative;
    height: 100vh;
    overflow: auto;
}

.search-section {
  ...
  ...
  top: 150px; 
  ...
}
