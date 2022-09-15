## Code repository for "ClimateBERT: A Pretrained Language Model for Climate-Related Text"

Link to paper: [arxiv.org/abs/2110.12010](https://arxiv.org/abs/2110.12010)

## Usage
The usage is straightforward and comprises two steps: 

1. The tokenizer is augmented with potentially new tokens which represent climate change specific language. This step led to the inclusion of tokens such as 'CO2' or 'CH4' which are often key to properly representing text. The code for this step can be found in 'tokenizer_augmentation.ipynb'. Besides [transformer package](https://huggingface.co/), this step also requires the [transformers_domain_adaptation](https://github.com/georgian-io/Transformers-Domain-Adaptation) packages.
2. Using the augmented tokenizer, the next step is to train the language model. This step follows basic steps from [transformer package](https://huggingface.co/). We provide the code for this in 'language_modeling.ipynb'.

## Dependencies
Our code depends on the [transformer package](https://huggingface.co/) and on [transformers_domain_adaptation](https://github.com/georgian-io/Transformers-Domain-Adaptation). For training ClimateBert, we used transformer 4.20. and transformers_domain_adaptation 0.3.1.

## How do I cite ClimateBert?

For now, cite the [Arxiv paper](https://arxiv.org/abs/2110.12010):

```
@article{webersinke2021climatebert,
  title={Climatebert: A pretrained language model for climate-related text},
  author={Webersinke, Nicolas and Kraus, Mathias and Bingler, Julia Anna and Leippold, Markus},
  journal={arXiv preprint arXiv:2110.12010},
  year={2021}
}
```
