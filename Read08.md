# Forms and JS Events

## Forms

Forms allow you to collect information for the user of the website.
There are several types of forms.

- acton is the url location where data is sent to.
- textarea is used to create a multi-line text input.

### Checkbox example

                <form action="">
                    <p>How old are you?</p>
                    <input type="checkbox" name="age"
                    value="24">
                    <input type="checkbox" name="age"
                    value="30">
                    <input type="checkbox" name="age"
                    value="26">
                </form>

- use required="required" is used to make a inut required.

## Events

- element.onevent=functionName;
- element.addEventListener(event, function, false)
  [<== Back](README.md)
