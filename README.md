# BricsLang

The concept of a programming language: the absence of language words in the syntax.
``` JS
// Simple comparison condition
? a < b
  => a = a + b;

условие ? a<b && b==3, b
  => a++;

условие (123);

// Comparison condition
? a < b {
  a = a + b;
}
// Comparison condition, else
? (a < b) {
  a = a + b;
} : {
  a = 0;
}
// Comparison switch
! (123) {
  ! 321 : 
  ! 123 :
    a = 1;
  !:
    a = 0;
}
// Iterating through the array elements
& (array => item ) {
  print(item);
}
// Iterating through the numbers of the created array
& ([2...7] => item, i ) {
  print(item, i);
}
// Iterating over numbers in the range of 2-12 in increments of 3
& ([2...12:3] => item, i ) {
  print(item, i);
}
// The condition for Checking the presence of an element in an array
? (a => array) {
  print('A exist in array');
}
// The condition for Checking the index in an array
? (a -> array) {
  print('A exist in array');
}
? (array[a]) {
  print('A exist in array');
}
```

``` JS
// creating class 
myClass1 {
  propA;
  propB;
}
// creating function
myFunction1 (a, b) {
  a = a + b;
}

myClass2 {
  propA;
  propB;
  myFunction2 (a, b){
    a = 0;
  }
}

// Property hooks, also known as "property accessors" 
myClass3 {
  prop3;
  myFunction3 (method){
    ? method { // if the method is the content value, for set the value
      prop3 = 123;
    }
    : { // if method is empty value, for get the value
      !> prop3;
      // !> - Completion return sign
    }
  }
}
// Create (or copy) object "myObj3" from class "myClass3"
// And the names of the objects are always accessed by reference.
myObj3 = @ myClass3;    
myObj2.myFunction3 = 123;

```

``` JS
// arrays
arr = [1,2,3,4,6,7];
arr[] = 5;  // Add new number
arr[1];     // Get exist number 2 in position 1
arr[-2];    // Get exist number 6 in last position 2
arr();      // Get an entry with element and index from an array and moving the cursor to the next element
arr(23);    // Add new element in position in last array list and return etry with element and index 
arr.lenght; // Get length elements array
```









