## Weights and Biases

This is a tool to plot and analyse your model training using graphs and loss values. It keeps track of multiple training runs conducted, useful and handy to connect using API calls. The following is based on the playlist <www.youtube.com/watch?v=hmewPDNUNJs&list=PLD80i8An1OEGajeVo15ohAQYF1Ttle0lk>. Another tutorial source is <www.kaggle.com/code/samuelcortinhas/weights-biases-tutorial-beginner>

### 1. Install wandb and get API key
```bash
!pip install wandb -qU
import wandb
wandb.login()
```
Click on the link that comes up and paste the API key from it.

### 2. Create a wandb instance that takes in project name, parameters and creates a page on wandb website to track.

``` python
wandb.init(
      # Set the project where this run will be logged
      project="basic-intro", 
      # We pass a run name (otherwise it’ll be randomly assigned, like sunshine-lollypop-10)
      name=f"experiment_{run}", 
      # Track hyperparameters and run metadata
      config={
      "learning_rate": 0.02,
      "architecture": "CNN",
      "dataset": "CIFAR-100",
      "epochs": 10,
      })
```

### 3. Log metrics
```python
#Log metrics from your script to W&B
wandb.log({"acc": acc, "loss": loss})
```
All the metrics to log must be in the above dictionary.

### 4. Mark training run as finished
```python
wandb.finish()
```

