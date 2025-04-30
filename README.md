# BricsLang

The concept of a programming language: the absence of language words in the syntax.
``` JS
// Simple comparison condition
?? a < b a = a + b;

// Comparison condition
? a < b {
  a = a + b;
}
// Comparison condition, else
? (a < b) {
  a = a + b;
} :: {
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
myFunction2 (a, b) {
  a = a + b;
}

myClass2 {
  propA;
  propB;
  myFunction3 (a, b){
    a = 0;
  }
}

// Property hooks, also known as "property accessors" 
myClass2 {
  prop3;
  myFunction3 (method){
    ?? method { // if the method is the content value, for set the value
      prop3 = 123;
    }
    ?! method { // if method is empty value, for get the value
      !> prop3;
      // !> - Completion return sign
    }
  }
}

myObj2 = @ myClass2;
myObj2.myFunction3 = 123;

```

``` JS
// arrays
arr = [1,2,3,4,6,7];
arr[] = 5;  // add new number
arr[1];     // Get exist number 2 in position 1
arr[-2];    // Get exist number 6 in last position 2
arr();      // Get an entry with element and index from an array and moving the cursor to the next element
arr(23);    // Add new element in position in first array list
```









