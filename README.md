# DP-with-normalized-class-representatives

This is an ongoing research project. We investigate the release of one frozen embedding (or more?) per class and create a simple model to predict labels for new data instances. Each sample is classified to the class representative with the highest cosine similarity, which takes an extremely short time compared to training a new classifier with differential privacy on top of the frozen embeddings. The simplicity of this approach allows for theoretical investigations as well. 

We have focused our attention on frozen pretrained models (SimCLR, Dino, etc.) that directly encourage higher cosine similarity between similar concepts. The normalization of features in such models discards the need for vector clipping, as each embedding is projected to the unit hypersphere by default. Our preliminary results are very promising, and we are continuing our experiments to be able to write a nice paper and publicly release the full code.


This research project is a part of my work at the DML laboratory at Sharif University of Technology under the supervision of Prof. Rabiee. and Gita Sarafraz. I wrote all of the code myself. Also, all of the main current ideas were developed by me. For inquiries, email me at amirmm379@gmail.com 
