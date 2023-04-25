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
 * ```.getQuery()```does not have an input but the output does change according to whatever is after the `?` in the URL, ```.split()``` argument does not change because the code is attempting to split the queries up by =.

***

## Part 2
Failiure
```
  @Test
  public void testReverseinPlace2() {
    int[] input1 = {1, 2, 3};
     ArrayExamples.reversed(input1);
    assertArrayEquals(new int[]{3, 2, 1}, input1);
  }  
```
No Failure
```
	@Test 
	public void testReverseInPlace() {
    int[] input1 = { 3 };
    ArrayExamples.reverseInPlace(input1);
    assertArrayEquals(new int[]{ 3 }, input1);
	}
 ```
Symptom

<img width="702" alt="image" src="https://user-images.githubusercontent.com/123005863/234182731-85a85d48-376a-4d53-a74a-cd80f2f0ae59.png">

Before
```
  static void reverseInPlace(int[] arr) {
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = arr[arr.length - i - 1];
    }
  }
```
After
```
  static void reverseInPlace(int[] arr) {
    for(int i = 0; i < arr.length/2; i += 1) {
      int temp = arr[i];
      arr[i] = arr[arr.length - i - 1];
      arr[arr.length -i-1] = temp;
    }
  }
```

## Part 3
words
