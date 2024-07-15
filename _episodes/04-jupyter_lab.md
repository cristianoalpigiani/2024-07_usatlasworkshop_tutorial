---
title: "JupyterLab"
teaching: 0
exercises: 0
questions:
- "What is JupyterLab?"
objectives:
- "Learn: number of GPU instances, selecting a Docker image and GPU memory"
keypoints:
- "Check JupyterLab documentation"
---

Users can deploy one or more private JupyterLab applications.

To encourage fair sharing these applications are time limited. 

## Selecting a number of GPU instances
> ## Number of GPU instances
>
> - The AF cluster has four NVIDIA A100 GPUs. 
>
> - GPU partitioned into -> seven GPU instances.
>
> - AF cluster can have up to 28 GPU instances running in parallel.
>
> - **You can select anywhere from 0 to 7 GPU instances as resources for the notebook.**
>
{: .callout}

Selecting Docker image
> ## 2 image options
>
> - 1: full anaconda (ivukotic/ml_platform:conda)
>
> - 2: NVidia GPU and ROOT support (ivukotic/ml_platform:latest)
>   - This one has ML packages (Tensorflow, Keras, ScikitLearn,...) preinstalled, check /ML_platform_tests tutorial
> 
{: .callout}

For software additions and upgrades please contact ivukotic@uchicago.edu

Selecting GPU memory

Select 40,836 MB for an entire A100 GPU. Select 4864 MB for a MIG instance.

You can learn more about in its  <a href="https://jupyterlab.readthedocs.io/en/stable/user/interface.html">JupyterLab</a> documentation link

{% include links.md %}

