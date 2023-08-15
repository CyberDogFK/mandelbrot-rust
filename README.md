Draw pretty beautiful mandelbrot pics

Usage:
cargo build --release

target/release/mandelbrot mandel.png 40000x30000 -1.20,0.35 -1,0.20
or interesting foundings
target/release/mandelbrot mandel.png 100000x90000 -1.20,0.35 -1,0.20
target/release/mandelbrot mandel.png 100000x90000 -0.90,0.95 1,-0.50
target/release/mandelbrot mandel.png 10000x9000 -1.55,1 -0.5,-1.5
target/release/mandelbrot mandel.png 1000x900 -2.55,1 -0.5,-1.5
target/release/mandelbrot mandel.png 1000x900 1.55,-1 -1.90,1
target/release/mandelbrot mandel.png 1000x900 0.666,1.666 -1.666,-0.666

as i mention we have (x1, y2) and (x2, y2) so
If we increase x1 we move image to right corner
if we decrease x2 we move image to left corner
If we decrease y1 we move image to below line
If we increase y2 we move image to upper line

if we change sign of values(they still musts be opposite, (mean, if x1 > 0, then x2 < 0)) directions stays

You could run with 'time' unix command to check multithreading
Also, in main method, you can change number of threads, best -is that, what equal to number of physical cores(also, maybe, i would add some create to make it auto)
