# Jexpresso tutorials <img src="https://github.com/EXPRESSOLAB/Jexpresso.jl/blob/master/assets//logo-ext2.png" width="40" title="Jexpresso logo">

*Solve systems of conservation laws in Julia using high order spectral elements*


| **Documentation** |
|:------------ |
| [![](https://img.shields.io/badge/docs-stable-blue.svg)](https://smarras79.github.io/Jexpresso/dev/) [![](https://img.shields.io/badge/docs-dev-blue.svg)](https://Jexpresso.github.io/Tutorials/dev)  |
|**Build Status** |
| [![CI](https://github.com/smarras79/Jexpresso/actions/workflows/CI.yml/badge.svg?branch=master)](https://github.com/smarras79/Jexpresso/actions?query=workflow%3ACI)
| **Contacts**  |
| [![Simone Marras](https://img.shields.io/badge/Simone%20Marras-smarras%40njit.edu-8e7cc3)](mailto:smarras@njit.edu) |
| [![Yassine Tissaoui](https://img.shields.io/badge/Yassine%20Tissaoui-yt277%40njit.edu-8e7cc3)](mailto:yt277@njit.edu) |
| [![Hang Wang](https://img.shields.io/badge/Hang%20Wang-hang.wang%40njit.edu-8e7cc3)](mailto:hang.wang@njit.edu) |
| **Citation** |
| [![DOI](https://img.shields.io/badge/article-arXiv:2401.05624-green)](https://doi.org/10.48550/arXiv.2401.05624) |


## What

This repo contains a set of tutorials to learn how to solve systems of conservation laws using the Julia library Jexpresso. 
At the root of this ecosystem is the [Jexpresso.jl](https://github.com/EXPRESSOLAB/Jexpresso.jl) library. 
The initial tutorials illustrate the usage of the tools in [Jexpresso.jl](https://github.com/EXPRESSOLAB/Jexpresso.jl), and these are the tutorials new users should focus on.

Within the Jexpresso ecosystem there are several [satellite/plugin packages](https://github.com/EXPRESSOLAB/Jexpresso.jl#plugins) that serve different purposes. Some of the tutorials focus on the combined usage of [Jexpresso.jl](https://github.com/EXPRESSOLAB/Jexpresso.jl) and the plugin packages. For example, [this tutorial](https://Jexpresso.github.io/Tutorials/dev/pages/t016_poisson_distributed/) illustrates the usage of [JexpressoDistributed.jl](https://github.com/Jexpresso/JexpressoDistributed.jl) for the solution of PDEs on parallel distributed-memory supercomputers.

The tutorials are available in two formats:

- As jupyter notebooks, allowing an interactive learning experience. **This is the recommended way to follow the tutorials**

- As HTML pages, allowing a rapid access into the material without the need of any setup.

## How

Visit one of the following pages, depending of your needs, and start enjoying!

- [**DEVEL**](https://Jexpresso.github.io/Tutorials/dev) &mdash; *Tutorials for the in-development version of Jexpresso.jl.*

## Generating tutorials locally 

Note: **only if you intend to contribute to the tutorials as an advanced user/developer**

If you want to contribute to the tutorials, e.g., to make changes in their sources, you might need to generate (render) them locally to see whether the changes in the sources produce the expected outcome in the output (i.e., Jupyter notebooks + HTML pages). To this end, you have to follow the following instructions once:

```
julia --project=docs   # From the Unix shell, located at the root of Tutorials repo 
develop .              # From the Julia package manager prompt
instantiate            # "" 
build                  # "" 
exit()                 # From the Julia REPL
```

and then, each time that you perform a change on the tutorial sources, you have to execute the following command:

```
julia --project=docs docs/make.jl # From the Unix shell, located at the root of Tutorials repo 
```

to generate the tutorials. The files generated are available at `Tutorials/docs/build/`. 


## How to cite Jexpresso

In order to give credit to the `Jexpresso` contributors, we simply ask you to cite the reference below in any publication in which you have made use of `Jexpresso` packages:

```
@article{tissaoui2024,
  author = {Y. Tissaoui and J. F. Kelly and S. Marras}
  title = {Efficient Spectral Element Method for the Euler Equations on Unbounded Domains},
  volume ={487},
  pages={129080},
  year = {2024},
  journal = {App. Math. Comput.},
}
```

## Contacts

[Simone Marras](mailto:smarras@njit.edu), [Yassine Tissaoui](mailto:yt277@njit.edu), [Hang Wang](mailto:hang.wang@njit.edu)





