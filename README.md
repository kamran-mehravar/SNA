# SNA
SNA-unipi
spreading:
simulate ,using the "NDlib" python library ,the diffusion models discussed during the course (SI,SIS,SIR,Threshol model) both on the crawled data on synthetic graphs (ER and VA).
Analyse the simulation  results varying boath model parameters  and initial conditions().

For running the code you must use this Website as a laboratory because it needs a lot of resources for running
the website is https://colab.research.google.com/ .
 
 for the Projection part, you have to upload the dataset from the beginning of the running.
 in addition for another part, you have to after the running projection section, results Must be collected and replace as values of the Network Definition.
 for instance, you can do like this: g=nx.erdos_renyi_graph(11110,226.9941/11110), the 11110 and 226.9941/1110 are the results from the projection part, also these values depend on our results per running, this is simply because the code select nodes and edges by random. 
