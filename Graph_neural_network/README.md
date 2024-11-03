<www.youtube.com/watch?v=A-yKQamf2Fc> and <www.youtube.com/watch?v=A-yKQamf2Fc>, <www.datacamp.com/tutorial/comprehensive-introduction-graph-neural-networks-gnns-tutorial>
## Graph Neural Network

Neural Networks find relationships between input data and output data, i.e a fn. that maps the input and output. The input data used for neural networks are predominantly structured data be it numbers, images(matrix of pixelated no.s) or sentences(string of embeddings). 
## Idea:
If the relationship between two variables say (x=2y or x = 2  *y + 0) is expressed as a linear combination b/w variables,then why can't social media and other graph structures which historiacally solved using linear algebra be solved using NNs?

In convolution NNs, each pixel is mapped with its neighbouring pixels to create a represention(output of convolution based) and as we have sufficient layers, each portion of image's localised information is represented in the final output. Now for graphs, each node has a certain relation to its neighbouring nodes so if we have an operation like convolution to repetitively share the info/properties of each node, then after some rounds(equivalent to no.of layers in NN), we can accurately map the relationships in a graph.

Introductory video of how this is achieved is given in <www.youtube.com/watch?v=GXhBEj1ZtE8>