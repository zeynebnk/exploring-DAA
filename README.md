# exploring-DAA
How many data points is a synthetic data point worth? Wuantifying the downstream impact of data.
Reference to the full paper: https://aclanthology.org/2023.loresmt-1.8/

DAA (Data Augmentation Advantage) is computed based on a linear interpolation of a baseline model, where x is the amount of data and y is the downstream performance.
For a specific target score b:

  Let xt be the number of training pairs needed to achieve b in the current experiment (with synthetic data)
  
  Let xb be the number of training pairs needed to achieve b in the baseline model (without synthetic data)
  
Calculate xadv (the advantage) as: xadv = xb - xt

Finally, DAA is calculated as: DAA = xadv/xt

In our analyses, we observe the **value of synthetic data** generated through various approaches, identifying key approaches and their effectiveness with different amounts of data and different tasks. We further show the importance of **diversified data** and the noise-quality trade-off, as well as the role of **quality** over **quantity** of data. 

This can be expanded to different tasks to understand the role of data in AI.
