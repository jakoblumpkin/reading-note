# State and Props


copied from 
https://reactjs.org/docs/state-and-lifecycle.html

                function Clock(props) {
                  return (
                    <div>
                      <h1>Hello, world!</h1>
                      <h2>It is {props.date.toLocaleTimeString()}.</h2>
                    </div>
                  );
                }

                function tick() {
                  ReactDOM.render(
                    <Clock date={new Date()} />,
                    document.getElementById('root')
                  );
                }

                setInterval(tick, 1000);

                function tick() {
                  const element = (
                    <div>
                      <h1>Hello, world!</h1>
                      <h2>It is {new Date().toLocaleTimeString()}.</h2>
                    </div>
                  );
                  ReactDOM.render(
                    element,
                    document.getElementById('root')
                  );
                }

                setInterval(tick, 1000);

                class Clock extends React.Component {
                  render() {
                    return (
                      <div>
                        <h1>Hello, world!</h1>
                        <h2>It is {this.props.date.toLocaleTimeString()}.</h2>
                      </div>
                    );
                  }
                }


                constructor(props) {
                  super(props);
                  this.state = {date: new Date()};
                }



[<== Back](README.md)