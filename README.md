# Shortest Path Distance Approximation

## Project Structure
The project structure of our group work is as depicted in the following tree structure.


    ├── final 
        ├── douban 
	        ├── datasets 		 
	        ├── embeddings 		# the embeddings for the graph 
	        └── douban_edges.txt	# the edgelist of a graph 
	    ├── facebook
	        ├── datasets 		# a folder containing different datasets generated for different landmark approaches 
	        ├── embeddings 		# the embeddings for the graph 
	        └── facebook_edges.txt	# the edgelist of a graph 
        ├── embedding_optimization 
	    ├── src 
	        ├── Dataset_Generation.ipynb 		# a folder containing different datasets generated for different landmark approaches 
	        ├── Embedding_generation.ipynb 		# the embeddings for the graph  
	        └── GA_DL_base_implementation.ipynb	# the edgelist of a graph 
    ├── preperations             
    └── README.md 
The project is divided into `final` and `preparations`. For the submission, only the final folder is of relevance, as the preparation folder only includes files that were used for meetings before, like images of the graph, earlier results, etc. The final folder includes three folders for the three datasets, we collected/tried to get results for. Inside these folders one can find generated datasets through multiple landmark approaches, the embeddings for the corresponding graph and the graph itself as an edgelist. Also, in the embedding_optimization folder, there is a small notebook that was used to extract information from log files that were needed for embedding optimization.

Overall, in the `src` folder, one can find the complete implementation in `GA_DL_base_implementation.ipynb`. There, one can see the complete code that was used for embedding generation, dataset generation through landmark approach, model creation and results collection, as well as optimization of embeddings. 

However, for further efficiency (parallel runs of embedding creation, dataset generation and result collection), we divided the code into multiple files. We extracted code from the base implementation into three main parts. `Embedding Generation`, `Dataset Generation` and `Results_collection_%dataset%`. These parts mainly include the same code as in the base implementation but were refractored for modularity reasons. In every Results collection file per graph (facebook, douban, youtube), one can find the code for creating a regression model for the task of Shortest Path Distance Approximation and code that collects results and plots. 
