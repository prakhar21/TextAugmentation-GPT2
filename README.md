# TextAugmentation-GPT2
Fine-tuned pre-trained GPT2 for topic specific text generation. Such system can be used for Text Augmentation.

## Getting Started
1. git clone https://github.com/prakhar21/TextAugmentation-GPT2.git
2. Move your data to __data/ dir__.

## Tuning for own Corpus
1. Assuming are done with Point 2 under __Getting Started__
```
2. Run python3 train.py --data_file <filename> --epoch <nunber_of_epochs> --warmup <warmup_steps> --model_name <model_name>
```

__Note:__ First time you run, it will take considerable amount of time because of the following reasons - 
1. Downloads pre-trained gpt2-medium model  _(Depends on your Network Speed)_
2. Fine-tunes the gpt2 with your dataset _(Depends on size of the data, Epochs, Hyperparameters, etc)_

All the experiments were done on [IntelDevCloud Machines](https://software.intel.com/en-us/devcloud)
