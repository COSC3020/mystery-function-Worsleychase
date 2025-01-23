# Mystery Function

What does the `mystery()` function in the following piece of code do? Add your
answer to this markdown file.

```javascript
function mystery(a) {
    if(a.length == 1) return a[0];
    var foo = mystery(a.slice(1, a.length))
    if(foo > a[0]) return foo;
    else return a[0];
}
```
Answer:

If the input (a) is an array of length 1, it will return the first/zero-th element of the array.
Otherwise, intialize a variable 'foo' that recursively calls mystery but essentially trims the array by 1 from the front, so it removes the first/zero-th element.
If the current element (foo) being iterated over (see line above) is greater than the first element (that is slowly being remove), return it.
Otherwise, return the first element.
In essence this just returns the largest element of a list using recursion.

Resources used:
https://www.w3schools.com/Jsref/jsref_slice_array.asp

I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice.
