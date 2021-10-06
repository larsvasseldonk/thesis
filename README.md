# Thesis

Title: **From a Monolith to Microservices: The Effect of Multi-view Clustering**
University: Utrecht University
Year: 2021
Author: Lars van Asseldonk
Supervisor: Dr. J. (Jurriaan) Hage

## Abstract

In today's demanding world, many companies migrate their monolithic systems to a microservices landscape. The most costly task in this process is refactoring the application into a suitable set of microservices. Decomposition techniques help the architect to understand better how the intended microservices architecture can be designed. These techniques take the monolithic system as input and output a set of candidate microservices. Over the years, many microservice decomposition techniques have been proposed. 
Most of these techniques focus on one viewpoint of the system, such as its static or dynamic behaviour, even though it is perfectly possible to combine them. 
To the best of our knowledge, we did not find any research that measures the effect of incorporating multiple viewpoints of the system on the quality of the microservices decomposition. 
This thesis studies the effect of multiple viewpoints based on the rationale that extra information results in a better decomposition. To do this, we developed a Python tool that extracts static, semantic, and dynamic dependencies from a monolith and represents them in an edge-weighted graph. 
A graph algorithm (Louvain) is then used to find communities in the graph that are highly connected and loosely coupled. We validate our approach by applying our tool to seven open-source Python projects. The quality of the resulting decompositions is then measured and compared in terms of functional independence and structural and conceptual modularity quality. The results show that incorporating multiple views of the system does not gradually increase the quality of the decomposition. However, combining static and dynamic information does result in a better decomposition in terms of modularity quality compared to the use of static or dynamic information individually. When semantic information is involved, we noticed that the decomposition quality significantly decreases for three metrics (IFN, OPN and, SMQ). 
This pattern could be justified by the fact that semantic decompositions contain much more dependencies, and therefore tend to favor semantics while focussing less on static and dynamic dependencies.

In the `analysed-projects` folder, the data used for the master thesis 'From a Monolith to Microservices: The Effect of Multi-view Clustering' is given. The `latex-files` folder contain all the .Tex files to create 
