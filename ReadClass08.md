# APIs
copied from https://medium.com/factory-mind/regex-tutorial-a-simple-cheatsheet-by-examples-649dc1c3f285

copied from https://visionmedia.github.io/superagent/
        request.post('/user')
            .send({ name: 'tj' })
            .send({ pet: 'tobi' })
            .then(callback, errorCallback)

             request
              .get('/search')
              .query({ query: 'Manny' })
              .query({ range: '1..5' })
              .query({ order: 'desc' })
              .then(res => {

              });
            Character classes — \d \w \s and .
            \d         matches a single character that is a digit -> Try it!
            \w         matches a word character (alphanumeric character plus underscore) -> Try it!
            \s         matches a whitespace character (includes tabs and line breaks)
            .          matches any character -> Try it!


[<== Back](README.md)