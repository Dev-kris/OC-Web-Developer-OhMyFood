# OC-Web-Developer-OhMyFood

This project was designed to challenge typical usage of CSS3. As such this project is built using only HTML and CSS, no JS was allowed. 
This was a mobile-first development with no mock for tablet, laptop, or desktop versions.

The majority of this site used flexbox and responsive versions used a combination of grid and flexbox.

### What was challenged?

Specifically, this website needed to include animations and effects that are typically accomplished by simple JS.
<img align="right" src="https://raw.githubusercontent.com/Dev-kris/OC-Web-Developer-OhMyFood/main/images/site-animations.gif">
### Animations
1. Loading screen upon initial site load/refresh and when navigating to each page.
  This is a proof of concept element that partially obscures the website and displays a loading animation.
  Both the page cover and the loading element need to dissapear both visually and to any possible interactions. 

2. Hover fill of icons, specifically a heart icon.
  Having an icon change colors and fill on :hover or :active is easier said than done, especially to make it visually appealing. 
  The most likely method used would be to stack font awesome icons to have a heart outline in black and a (hidden) filled heart of the desired color.
  This then introduces potential issues of alignment, increased number of classes, and an animated effect that leaves something to be desired.
  The solution to this was to have just one icon and apply a -webkit-stroke effect to outline the icon in the desired visible color. 
  This simplified the code and allowed fine tuning of the icon outline thickness.
  
3. Hover affect on menu items.
  Inside each restaurant page contains a selection of menu items. These items, when hovered over or clicked, would animate a small checkbox on the right side.
  This effect would move the text within the element and text overflow would be hidden with elipses. 
  This was accomplished using flexbox for the main card and an element with a width of 0 (which changed on :hover).
  The rotating check mark was made using a fontawesome icon with a animated transform rotate(360).

4. Menu items entry effect (float in).
  Client wanted the menu items to float in upon page loading. This is currently linked to a set delay due to the limitations of css.
  Effect was achieved using keyframes with a translateY effect. 
  
### Live version

Live version can be found on Github Pages. https://dev-kris.github.io/OC-Web-Developer-OhMyFood/
