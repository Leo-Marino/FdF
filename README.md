# FDF
This program generates a wireframe model representation of a 3D landscape from a text file by appliyng the Bresenham algorithm to calculate wich pixels must be colored in order to produce the corresponding image

## Instructions
### Makefile :wrench:
Extracts the graphical library from the compressed file, compiles the program and generate executable file:

	make

Remove object files:

	make clean

Remove objects, executable and the extracted minilibx folder:

	make fclean

Remove compilation products and compile again:

	make re

### Launch 🚀
Run from terminal the executable file (fdf) along with a valid map file:

	./fdf maps/42-col.fdf

### Commands 🕹️
Traslate the image:

	Arrow keys

Zoom in:

	'r'

Zoom out:

	'f'

Rotate on x axys:

	'a' & 'd'

Rotate on y axys:

	'w' & 's'

Rotate on z axys:

	'q' & 'e'

Close session:

	'Esc' or 'Delete'

### Map File 🗺️
A valid map file must follow this format:\

	The file name needs to have the ".fdf" extension at the end of it's name

Each number will represent a point on the base grid;\
Decimal numbers indicate the height of the point:

	0 0 0 0 0

Heights can be followed by an hexadecimal number to define the color of the corresponding line:

	0  0 10,0xFF0000 10,0xFF0000  0
