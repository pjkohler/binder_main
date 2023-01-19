This repo is used to define an environment for generating Binder demos used by the [Kohler Visual Neuroscience Lab](https://www.kohlerlab.com/) at York University.

A binder hub link can then be generated here: https://jupyterhub.github.io/nbgitpuller/link

where binder_main (this repo) is the environment repo and any other repo is the content repo. I have created a mostly empty repo, [binder_test](https://github.com/pjkohler/binder_test) that can be used as the content repo for testing purposes. 

The idea is that the environment is hosted separately from the content, which means that changes to the content can be made without necessitating a reload of the environment. I find this helps immensely, as the environment is often specified from the beginning, while changes to the content are many and often. 

This is expressed in more detail in this [forum post](https://discourse.jupyter.org/t/tip-speed-up-binder-launches-by-pulling-github-content-in-a-binder-link-with-nbgitpuller/922) by [@choldgraf](https://github.com/choldgraf).

The environment defined here currently includes:

- numpy
- seaborn
- scipy
- pip
- nbgitpuller (required)
- pandas
- matplotlib
- nilearn
- osfclient
- psignifit, hosted here: https://github.com/wichmann-lab/python-psignifit
