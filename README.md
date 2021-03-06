## Software for Simulation of Flat Trusses in python

This software was developed for a subject called heat transfers and solids mechanics, from the computer engineering course at Insper. The main idea was to input the characteristics of a structure such as a bridge, using a table and to generate support reactions, nodal displacements, deformations, internal forces and internal stresses as an output using the finite element method.

The file "funcoesTermosol.py" was provided by the teachers of the discipline, with functions in Portuguese to assist in receiving the information and generating the output graph.
The file "contest.py" contains the structure to be analyzed, which can be viewed below:


![Structure image](/assets/structure.jpeg)


The file "flatTrussSimulator.py" is used to run the software itself. You will need to select the method available for solving the system of differential equations (Gauss-Seidel or Jacobi) using an input and after that, you will have the results generated by the algorithm.

The result for the "context.xlsx" structure is saved in the "output.txt" file and can be viewed below:


![Result image1](/assets/result1.png)
![Result image2](/assets/result2.png)



The software was developed by Caio Fauza, Pedro Paulo Telho and Luiz Vitor Germanos.


## Structure collapse
  
In the software there is a function to analyze the collapse of the structure, which was defined by:

 - Some member has exceeded the tensile strength of 18 MPa
 - Some member exceeded the compressive tensile strength of 18 MPa
 - Some member had a deformation greater than 5%
 - Some node moved more than 20mm in X or Y
 
 You can use the function by calling:
 > checkCollapse()
