# FUNCTIONAL PROGRAMMING

            // Unrefactored code

            const URLstore = [];

            function makeShort(URL) {
              const rndName = Math.random().toString(36).substring(2);
              URLstore.push({[rndName]: URL});
              return rndName;
            }

            function getLong(shortURL) {
              for (let i = 0; i < URLstore.length; i++) {
                if (URLstore[i].hasOwnProperty(shortURL) !== false) {
                  return URLstore[i][shortURL];
                }
              }
            }

          // Refactored code
          function makeShort(URL) {
            const rndName = Math.random().toString(36).substring(2);
            // Place the short URL into the Map as the key with the long URL as the value
            URLstore.set(rndName, URL);
            return rndName;
          }

          function getLong(shortURL) {
            // Leave the function early to avoid an unnecessary else statement
            if (URLstore.has(shortURL) === false) {
              throw 'Not in URLstore!';
            }
            return URLstore.get(shortURL); // Get the long URL out of the Map
          }

[<== Back](README.md)