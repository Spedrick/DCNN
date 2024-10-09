# DCNN
An implementation of [Diffusion-Convolutional Neural Networks](http://papers.nips.cc/paper/6212-diffusion-convolutional-neural-networks.pdf) [1] in Theano and Lasagne.

## Installation
    git clone https://github.com/Spedrick/dcnn.git
	cd dcnn

## Usage
### Node Classification (Cora)
	python -m client.run --model=node_classification --data=cora
### Graph Classification (NCI1)
	python -m client.run --model=graph_classification --data=nci1

## Code Structure
    client/: Client code for running from the command line.
      parser.py: Parses command line args into configuration parameters.
      run.py: Runs experiments.
    
    data/: Example datasets.
    
    python/: DCNN library.
      data.py: Dataset parsers.
      layers.py: Lasagne internals for DCNN layers.
      models.py: User-facing end-to-end models that provide a scikit-learn-like interface.
      params.py: Simple container for configuration parameters.
      util.py: Misc utility functions.

# Contributors

1. [Yuvraj Kumar | 2021IMG-066](https://github.com/Spedrick)
2. [Aman Tripathi | 2021IMG-005](https://github.com/meMANNY)
3. [Aakarshit Doda | 2021IMG-001]
(https://github.com/Aakarshit01)



# References
[1] [Atwood, James, and Don Towsley. "Diffusion-convolutional neural networks." Advances in Neural Information Processing Systems. 2016.](http://papers.nips.cc/paper/6212-diffusion-convolutional-neural-networks.pdf)

