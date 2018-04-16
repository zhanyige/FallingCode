FallingCode
=======================

### Introduction ###
Simulation of the scene of falling code on the terminal (which must be local, ssh remote terminal doesn't work).<br>


![alt text](http://cdn2-europe1.new2.ladmedia.fr/var/europe1/storage/images/europe1/culture/matrix-lorigine-du-code-vert-revelee-3478307/44949452-1-fre-FR/Matrix-l-origine-du-code-vert-revelee.jpg)

### Dependent library ###
ncurses<br>
If you want to use another library, you just need to edit `SysTool.cpp` and `makefile`.

### Installation ###
Download and execute `make`.

### Execution ###
Go to the directory `bin` and execute one of the commands as below:
* `./matrix.out colorValue`. E.g. `./matrix.out 23`.
* `./matrix.out string colorValue`. E.g. `./matrix.out "hello world!" 122`.
<br>Besides, the `colorValue` is optional and its range is [0, 255].


### additional... ###
I like to execute `./matrix.out` because the color by default is green.<br>

There is an issue left: I want to set a tail (with a different color) for each column, whose length is 0.3 * lengthOfColumn, but it would be a very heavy calculation (read the comment in the file Column.h) as it's about `double - multiplication`.<br>
My PC is a Mac Pro with 4GB RAM and its performance is not good enough so I comment the tail part. If you have another way to add the tail, it would be appreciated if you let me know.
