# Element Selector

The idea behind this was to save few lines of code and make DOM element traversing a bit less expensive. 
These functions use the concept of memoization to make a cache of DOM elements the first time js loads, 
afterwards DOM elements are returned from the cache. Also, you can use functions like map(), filter(), and forEach()
without the need to bind because it returns an array instead of NodeList.

# $getID()
  Arguments:
    1: id of DOM element
    2: true (if element is to fetched from cache) else false, [default: true].
    3: selector, [default: document]
# $getC()
  Arguments:
    1:  class of DOM element
    2:  true (if element is to fetched from cache) else false, [default: true].
    3:  'multiple' (if array of all elements having same class is required) else 'single', [default: 'single'].
    4:  selector, [default: document]
# $getQ() 
  Arguments:
    1:  query selector of DOM element (similar to document.querySelectorAll())
    2:  true (if element is to fetched from cache) else false, [default: true].
    3:  'multiple' (if an array of all elements having the same class is required) else 'single', [default: 'single'].
    4:  selector, [default: document]
