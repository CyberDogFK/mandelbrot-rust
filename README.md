Draw pretty beautiful mandelbrot pics

Usage:
cargo build --release

target/release/mandelbrot mandel.png 40000x30000 -1.20,0.35 -1,0.20
or interesting foundings
target/release/mandelbrot mandel.png 100000x90000 -1.20,0.35 -1,0.20
target/release/mandelbrot mandel.png 100000x90000 -0.90,0.95 1,-0.50

You could run with 'time' unix command to check multithreading
Also, in main method, you can change number of threads, best -is that, what equal to number of physical cores(also, maybe, i would add some create to make it auto)
