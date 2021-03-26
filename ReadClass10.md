# In memory storage

copied https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c
          (function testing(){
            function add(a, b) {
              try {
                var result = a + b
                return result.split('')
              } catch (error) {
                console.error('add went wrong ->', error)
                return [] // default value
              }
            }
            var stringResult = add("1", "2")
            var numberResult = add(1, 2)
          })()



          function firstFunction(){
           throw new Error('Stack Trace Error');
           }

            function secondFunction(){
              firstFunction();
            }

            function thirdFunction(){
              secondFunction();
            }

            thirdFunction();

[<== Back](README.md)