# Chart.js, Canvas

- Chart is a javaScript plugin.
- You downlaod chart.js
-            <script src="Chart.min.js"></script>

               <canvas id="" width="" height=""></canvas>

## Rectangular shape example

copied from

https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_shapes

-            function draw() {
                var canvas = document.getElementById('canvas');
                if (canvas.getContext) {
                    var ctx = canvas.getContext('2d');

                    ctx.fillRect(25, 25, 100, 100);
                    ctx.clearRect(45, 45, 60, 60);
                    ctx.strokeRect(50, 50, 50, 50);
                }
                }

- [<== Back](README.md)
