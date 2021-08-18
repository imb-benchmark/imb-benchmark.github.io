# Starting Guide
________________________________________________________________

## Quick overview over the process

The core of our OCPPS benchmarking is our provided package. 
It consists of a dataloader, who handles the download of our OCPPS datasets automatically as well as preprocess it. Subsequently to the processing of your model, OCPPS provides a standardized evaluator, that will display your achieved results. Afterwards send us your outstanding results within our e-mail template by the following [link](https://imb-benchmark.github.io//Contact.html).

![](C:\Users\Lukas Moddemann\Documents\Spaces\ML_Benchmark_Website\Arbeitspakete\Konzeptentwicklung\Markdown content\StartingGuide.png)



## Package installation

You can install our OCPPS package by using Python package manager pip.
> pip install ocpps 

#### ?If Updates are necessary? -> needs to be defined

> python -c "import OCPPS; print(OCPPS.__version__)"
> #Otherwise you should update your package by running
> pip install -U OCPPS

## Requirements -> needs to be defined
- Python >= 3.123
- PyTorch >= 1.123
- Numpy >= 2.234
- scikit-learn >= 2.123
- to be specified
_________________________________________________________________________________________

## Package handling
Through the OCPPS package you have access to an handy data loader and standardized evaluator for consistent comparability.
As an example there are stated some examples on our [imb-benchmark git](https://github.com/imb-benchmark?tab=repositories).

### Data Loader
Our developed OCCPS package consists of an handy data loader that performs dataset downloading and uniform dataset splits.

With the following example we want to show how to use our package by only using a few lines of code. 

> from OCPPS_package import something
> from torch.utils.data import DataLoader
>
> #Download data
> dataset = DownloadData(name = "name", root = 'dataset/')
>
> where_split = dataset.get_split()
> train_set = DataLoader(dataset[where_split["train"], batch_size=2, shuffle = True)
> valid_set = DataLoader(dataset[where_split["valid"], batch_size=2, shuffle = False)
> test_set = DataLoader(dataset[where_split["test"], batch_size=2, shuffle = False)


### Evaluator

Our package consists of standardized evaluators to test and compare submitted models for the benchmarking. The evaluator takes ***xxxx*** format as input and outputs a dictionary string that consists of performance metrics.

> from OCCPS_package import evaluator
>
> eval_model = Evaluator(name = "name")
>
> #input and output format can be figured out with the following lines of code
> #print(eval_model.expected_input)
> #print(eval_model.expected_output)
>
> input = {"y_true": y_true, "y_pred". y_pred}
> result = eval_model.eval(input)

# Citing

If you are writing a paper or in a different work and make references to OCPPS, please cite [our paper](https://imb-benchmark.github.io/).

***By now it's a book by Prof. Niggemann, but needs to be changed afterwards***

> @BOOK{Niggemann2018,
> AUTHOR = {Niggemann, Oliver AND Schüller, Peter},
> YEAR = {2018},
> TITLE = {IMPROVE - Innovative Modelling Approaches for Production Systems to Raise Validatable Efficiency - Intelligent Methods for the Factory of the Future},
> EDITION = {},
> ISBN = {978-3-662-57805-6},
> PUBLISHER = {Springer},
> ADDRESS = {Berlin, Heidelberg},
> }



