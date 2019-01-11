## Define closure?

<details>
    <summary>Answer here</summary>
     A closure means an inner function has access to the outer (enclosing) function’s variables—scope chain (even when outer function finishes execution). The closure has three scope chains: it has access to its own scope (variables defined between its curly brackets), it has access to the outer function’s variables, and it has access to the global variables.

     ```
      function buildFunctions() {

          var arr = [];

          for (var i = 0; i < 3; i++) {

              arr.push(
                  function () {
                      console.log(i);
                  }
              )
          }
          return arr;
      }

      var fs = buildFunctions();

      fs[0]();
      fs[1]();
      fs[2]();
     ```
</details>