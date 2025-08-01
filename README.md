# Uplift Model Evaluation with Ordinal Dominance Graphs </br><sub><sub>B. Verbeken, S. Verboven, W. Verbeke, M. Guery [[2025]](https://www.jmlr.org/papers/v26/22-1455.html)</sub></sub>

Uplift modelling is a subfield of causal learning that focuses on ranking entities by individual treatment effects. Uplift models are typically evaluated using Qini curves or Qini scores. While intuitive, the theoretical grounding for Qini in the literature is limited, and the mathematical connection to the well-understood Receiver Operating Characteristic (ROC) curve is unclear. In this paper, we introduce pROCini, a novel uplift evaluation metric that improves upon Qini in two important ways. First, it explicitly incorporates more information by taking into account negative outcomes. Second, it leverages this additional information within the Ordinal Dominance Graph framework, which is the basis behind the well known ROC curve, resulting in a mathematically well-behaved metric that facilitates theoretical analysis. We derive confidence bounds for pROCini, exploiting its theoretical properties. Finally, we empirically validate the improved discriminative power of ROCini and pROCini in a simulation study as well as via experiments on real data.

## Repository

This repository contains two notebooks:

- `uplift_metrics_algorithm1_simulation.ipynb`
 This is the **main notebook**. It contains:
  - The implementation of the uplift evaluation metrics used in the paper
  - The simulation code for **Algorithm 1**  
    (see [paper, p.6](https://www.jmlr.org/papers/volume26/22-1455/22-1455.pdf#page=6))


- `semisynthetic_experiment.ipynb`:  
  This notebook allows you to reproduce the **semi-synthetic experiment** described in **Section 4.2**  
  (see [paper, p.34](https://www.jmlr.org/papers/volume26/22-1455/22-1455.pdf#page=34)).  

## Installing
We have provided a `requirements.txt` file:
```bash
pip install -r requirements.txt
```
Please use the above in a newly created virtual environment to avoid clashing dependencies.

## Citing
Please cite our paper and/or code as follows:

```tex

@article{verbeken2025uplift,
  title={Uplift model evaluation with ordinal dominance graphs},
  author={Verbeken, Brecht and Guerry, Marie-Anne and Verbeke, Wouter and Verboven, Sam},
  journal={Journal of Machine Learning Research},
  volume={26},
  number={90},
  pages={1--56},
  year={2025}
}

```