# Servers and Bugs
## Part 1
My code for the ```String Server``` 

<img width="706" alt="image" src="https://user-images.githubusercontent.com/123005863/234175555-482ca9ca-ab3a-4484-a500-8d243fa58d3b.png">

***

Using ```/add-message``` 

<img width="538" alt="image" src="https://user-images.githubusercontent.com/123005863/234175626-67918e54-63bb-44f4-85a1-caf8855bf0a9.png">

<img width="641" alt="image" src="https://user-images.githubusercontent.com/123005863/234175671-5a588240-5a6e-42a5-8c13-e0c49e0a0e0b.png">

1. ``localhost: 4000/add-message?s=Hello``
  * This url calls a variety of methods, some of which are ``String.format()`` and ``.getPath()``.
  * The relevant argument for ``String.format()`` is ```msg```, which holds the message that will be printed out, in this case `"hello"`. For ```.getPath()```, the relevant argument is none as this method is meant only to retrieve a value, which in this the path after the domain.
  * In this case the field ```msg``` gets changed, as it started off as a blank string ```""``` which then after the the given path, was set to ```"Hello /n"```
2. ``localhost:4000/add-message?s=How%20are%20you``
 * Some other methods that are also called in this url are, ```.getQuery()``` and ```.split()```.
 * The relevant argument for ```.split()``` is ``"=''``, on the other hand, ```.getQuery()``` does not have a relevant argument because this method is only suppose to get what is after the `?` from the URL.
 * ```.getQuery()
***
## Part 2
words
## Part 3
words
