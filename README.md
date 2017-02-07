Website Performance Optimization portfolio project
==================================================

This project required improving the performance of loading and rendering an existing portfolio site. The speed of the site was measured using Chrome dev tools to identify performance bottlenecks, and then optimizations were applied to address those bottlenecks. In particular, the critical rendering path was optimised and this page was made to render as quickly as possible by applying the techniques, picked up in the [Critical Rendering Path course](https://www.udacity.com/course/ud884).

Getting started
---------------

####Part 1: Optimize PageSpeed Insights score for index.html
The live demo of this part can be found [here](https://riteshthakur961.github.io/frontend-nanodegree-mobile-portfolio/)

Optimisations made for this are:

1. Move scripts to the bottom.
2. Change external script loading to async.
3. Optimize images.
4. Minified & compresed html, js and css.
5. Inline CSS.
6. Add media = print for css/print.css.

####Part 2: Optimize Frames per Second in pizza.html
The live Demo for this part an be found [here](https://riteshthakur961.github.io/frontend-nanodegree-mobile-portfolio/views/pizza.html)

Optimisations made for this are:

1. Modfied the changePizzaSizes function to select randomPizzaContainer elements by class name (rather than querySelectorAll) and add them to a randompizzacontainer array.
2. Moved the computation of the dx and newwidth variables outside of the for loop as it doesn't seem necesary to recompute them on each pass through that loop.
3. Modified the updatePositions function to select the mover elements by class name.
4. Moved the access of the body.scrollTop property outside of the for loop.
5. Changed the number of pizzas generated on page load to be based on the browser window resolution.
6. Moved the querySelector call for selecting movingPizzas1 outisde of the for loop and saved it to a local variable called Pizzamoves.

Resources referenced:
---------------------

1. [Google Pagespeed Insight Rules:](https://developers.google.com/speed/docs/insights/rules)
2. [MDN docs on getElementsByClassName:]( https://developer.mozilla.org/en-US/docs/Web/API/Document/getElementsByClassName)
3. http://cssminifier.com/
4. https://imageoptim.com/
5. http://jscompress.com/