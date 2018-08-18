## Define inplace algorithm?

<details>
  <summary>Answer here</summary>
      ```javascript 
    function squareArrayInPlace(intArray) {
    intArray.forEach((int, index) => {
        intArray[index] *= int;
    });

    // NOTE: we could make this function return undefined,
    // since we modify intArray in place.
    return intArray;
    }

    function squareArrayOutOfPlace(intArray) {
    // We allocate a new array that we'll fill in with the new values
    const squaredArray = [];

    intArray.forEach((int, index) => {
        squaredArray[index] = Math.pow(int, 2);
    });

    return squaredArray;
    }```

  * An in-place algorithm operates directly on its input and changes it, instead of creating and returning a new object. This is sometimes called destructive, since the original input is "destroyed" when it's edited to create the new output
  But be careful: an in-place algorithm can cause side effects. 
  * Working in-place is a good way to save space. An in-place algorithm will generally have O(1)O(1) space cost.
  *  it means "without creating a new copy of the input." In general, an in-place function will only create additional variables that are O(1)O(1) space.

</details>