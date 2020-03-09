# Set-Structured Latent Representations 

## Software Requirements

This codebase requires Python 3, PyTorch 1.0+, Torchvision 0.2+. In principle, this code can be run on CPU but we assume GPU utilization throughout the codebase.

## Usage

The three files `run_reconstruct_circles.py`, `run_reconstruct_CLEVR.py` and `run_isodistance.py` correspond with the three main experiments in the paper.

Full usages:
```
usage: run_reconstruct_circles.py [-h] [--model_type MODEL_TYPE]
                                  [--batch_size BATCH_SIZE] [--lr LR]
                                  [--inner_lr INNER_LR]

optional arguments:
  -h, --help            show this help message and exit
  --model_type MODEL_TYPE
                        model type: srn | mlp
  --batch_size BATCH_SIZE
                        batch size
  --lr LR               lr
  --inner_lr INNER_LR   inner lr
```
```
usage: run_reconstruct_CLEVR.py [-h] [--model_type MODEL_TYPE]
                                [--batch_size BATCH_SIZE] [--lr LR]
                                [--inner_lr INNER_LR]

optional arguments:
  -h, --help            show this help message and exit
  --model_type MODEL_TYPE
                        model type: srn | mlp
  --batch_size BATCH_SIZE
                        batch size
  --lr LR               lr
  --inner_lr INNER_LR   inner lr
```  

```
usage: run_isodistance.py [-h] [--model_type MODEL_TYPE]
                          [--batch_size BATCH_SIZE] [--recon]
                          [--resume RESUME] [--lr LR]
                          [--weight_decay WEIGHT_DECAY] [--inner_lr INNER_LR]
                          [--save SAVE]

optional arguments:
  -h, --help            show this help message and exit
  --model_type MODEL_TYPE
                        model type: srn | mlp | cnn
  --batch_size BATCH_SIZE
                        batch size
  --recon               transfer models
  --resume RESUME       Resume checkpoint
  --lr LR               lr
  --weight_decay WEIGHT_DECAY
                        weight decay
  --inner_lr INNER_LR   inner lr
  --save SAVE           Path of the saved checkpoint
  ```
