# Passing Functions as Props

- If statement

          function BoilingVerdict(props) {
            if (props.celsius >= 100) {
              return <p>The water would boil.</p>;
            }
            return <p>The water would not boil.</p>;
          }

          ReactDOM.render(
            <BoilingVerdict celsius={1} />,
            document.getElementById('root')
          );






[<== Back](README.md)