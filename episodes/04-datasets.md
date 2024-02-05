---
title: Dataset Analysis With TopoStats
teaching: 30?
exercises: 20?
---

::::::::::::::::::::::::::::::::::::::: objectives

- Run TopoStats on an directory to obtain flattened images and geometric properties.
- Understand parameters in the configuration files and their effects.
- Understand what each of the metrics represent.

::::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::::::: questions

- How can I create, copy, and delete files and directories?
- How can I edit files?

::::::::::::::::::::::::::::::::::::::::::::::::::


## Perfecting the configuration parameters

### Step 1: Running a single image
Rather than re-running your whole dataset while fine tuning your TopoStats parameters, and spending a lot of time and computational resources to do so, you can gauge rough parameters by using a single image either via the terminal or Jupyter notebooks: 
1. Terminal - You can put an image into it's own folder, modfiy the `base_dir` field in the configuration file to point to it, and run TopoStats on the sole image. Additionally setting the `plotting.image_set` configuration parameter to `all` should allow you see at what individual stages the flattening parameters or grain finding parameters are failing in their respective folders.
2. Alternatively, the Jupyter Notebooks provided in the [TopoStats Github Repository](https://github.com/AFM-SPM/TopoStats.git) can walk you through each individual step and what it does to the obtained molecule masks.

### Step 2: Run TopoStats
With TopoStats installed, and our parameters fine-tuned to capture the molecules we want, 


### Step Z: Plot the aspect ratio



```
import pandas as pd
import seaborn as sns
base = "<path-to-file>/all_statistics.csv"
data = pd.read_csv(base)

data['topoisomer'] = data['basename'].str.strip().str[-1]
data['aspect_ratio'] = 1/data['aspect_ratio']

sns.violinplot(data, x='topoisomer', y='aspect_ratio', bw=0.1)
```


This chapter is from "[TopoStats][TopoStats]". It is licensed under the
[CC-BY-4.0][cc-by-4].


[Topostats]: https://swcarpentry.github.io/shell-novice/
[cc-by-4]: https://creativecommons.org/licenses/by-sa/4.0/
