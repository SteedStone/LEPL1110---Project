Finite Elements : LEPL1110
===========================

## Authors

- **Student:** Guerand Dewell
- **Student:** Romain Valadi

## How to launch the program 


To launch the program, follow these steps:

1. Ensure you have Python installed on your system (version 3.8 or higher).
2. Compile the makefile and the several exeutables :  
```
cmake CMakeList.txt 
make
```

3. Three executables are going to be created :

- ```myMesh``` : Create the mesh for the different geometry.
- ```myFem``` : Solve the problem.
- ```myVisualisation``` : Create a animation of the force acting on the structures.

### myMesh : 

Option :  
- Type de cartons (```1``` : Triangle ```2``` : Hexagone)
- Viualiser la forme (```1``` : Oui ```2``` : Non)
- Type de mailage (```0``` : Triangles ```1``` : Quadrilatères)
- Grand problème (```0``` : Non ```1``` : Oui)

Be careful after having generated the mesh please run ```python test.py```

### myFem : 

Option : 
- A file path to the mesh 

Option during compilation by pressing the following keys: 
- ```V``` : Default visualisation of the mesh with the deplacement (Mode geometry)
- ```S``` : Show the matrix (Mode matrix) 

In Matrix mode :
- ```F```: Show with a full solver 
- ```B```: Show with a band solver 
- ```X```: Renumerotation in X
- ```Y```: Renumerotation in Y
- ```N```: No Renumerotation 

In Geometry mode : 
- ```X```: Show the forces in X 
- ```Y```: Show the forces in Y
- ```K```: Show the Sigma in X
- ```L```: Show the Sigma in Y
- ```T```: Show the Node that "break"




### myVisualisation : 

To compile the visualisation please enter : 
```make video```
