# Element Selector

> The idea behind this was to save few lines of code and make DOM element traversing a bit less expensive. 
> These functions use the concept of memoization to make a cache of DOM elements the first time js loads, 
> afterwards DOM elements are returned from the cache. Also, you can use functions like map(), filter(), and forEach()
> without the need to bind because it returns an array instead of NodeList.

## $getID()
  Arguments:
    - id of DOM element
    - true (if element is to fetched from cache) else false, [default: true].
    - selector, [default: document]
## $getC()
  Arguments:
    -  class of DOM element
    -  true (if element is to fetched from cache) else false, [default: true].
    -  'multiple' (if array of all elements having same class is required) else 'single', [default: 'single'].
    -  selector, [default: document]
## $getQ() 
  Arguments:
    -  query selector of DOM element (similar to document.querySelectorAll())
    -  true (if element is to fetched from cache) else false, [default: true].
    -  'multiple' (if an array of all elements having the same class is required) else 'single', [default: 'single'].
    -  selector, [default: document]
