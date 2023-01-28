# Token-Level Reward-Policy Learning for Sequence Generation

This is a preliminary release of the source codes associated with the paper.
A cleaner version will be released once available.

## Dependency

To install the required packages, please execute the following command:
```angular2html
bash install_packages.sh
```

## Experiments

### Prompt Experiments

To reproduce the prompt experiments on the `sst-2` dataset under `dataset_seed=0` and `random_seed=0`, 
please use the following commands
```angular2html
cd prompt_task/examples/few-shot-classification
python run_fsc.py
```
Please check `fsc_config.yaml` for available flags.

For experiments on the `agnews` dataset, please change the corresponding flags in `fsc_config.yaml` accordingly. 

### Summarization Experiments
To run the summarization experiments under random seed `0`, please use the following commands
```angular2html
cd sum_task/

# for the "cnn_dailymail" dataset 
python run_sum.py --dataset_name="cnn_dailymail" --dataset_config="3.0.0" --seed=0

# for the "xsum" dataset
python run_sum.py --dataset_name="xsum" --seed=0
```

## Acknowledge

This codebase builds on the following codebases:
* [**RLPrompt**](https://github.com/mingkaid/rl-prompt)
* [**HuggingFace Summarization Example**](https://github.com/huggingface/transformers/tree/main/examples/pytorch/summarization)




















