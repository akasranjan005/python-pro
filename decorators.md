# Python Decorators

````
from time import time
def timer(func):
  def f(x,y=10):
    before=time()
    rv=func(x,y)
    after=time()
    print "elapsed time: ",after-before
    return rv
  return f

@timer
def add(x,y=10):
  return x+y
````

This is one of the most easiest example that i came across.
