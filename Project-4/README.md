//testing and comparing iota.cpu vs iota.gpu

From what I can tell with the comparisons of the cpu vs gpu is that the cpu does the computation faster even though it is a very simple computation thats 
happening. The reason why it is important to notice is because, since it is so simple, the overhead that's occuring as the transfer of data from cpu to gpu
memory, it ends up dominating the total run time. The reason why this is happening is because there really isn't a purpose to the data transfer that calls for the use of the gpu hence why its increasing so much.


 
