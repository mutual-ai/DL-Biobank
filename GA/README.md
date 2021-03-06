# Evolve a neural network with a genetic algorithm

This is an code used to find the optimal network parameters for trait regression task. 
It's  a fork of [Jan Liphardt's implementation, DeepEvolve](https://github.com/jliphard/DeepEvolve) to work with MLPs and CNNs. It uses the Keras library to build, train and validate.

For more, see this blog post: 
https://medium.com/@harvitronix/lets-evolve-a-neural-network-with-a-genetic-algorithm-code-included-8809bece164

## To run

#### Optimize MLPs architecture for Height with 10k Best SNPS 
```python main.py --mlp```

#### Optimize CNNs architecture for BHMD with 10k Best SNPS 
```python main.py --cnn --trait BHMD```


## Credits

The genetic algorithm code is based on the code from this excellent blog post: https://lethain.com/genetic-algorithms-cool-name-damn-simple/ and this excelent repository: https://github.com/rileymcdowell/genomic-neuralnet

It's a fork of [Jan Liphardt's implementation, DeepEvolve](https://github.com/jliphard/DeepEvolve) 

## Using it with your own data
Modify the function ```utils.retrieve_data``` so it loads your data and returns it in a numpy.ndarray with SNPS as columns

## Contributing

Have an optimization, idea, suggestion, bug report? Pull requests greatly appreciated!

## License

MIT
