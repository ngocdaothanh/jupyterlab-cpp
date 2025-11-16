# JupyterLab with C++ kernel in Devbox

See:
- https://jupyter.org
- https://www.jetify.com/docs/devbox/devbox-examples/languages/python

## Install Nix packages

Install [Devbox](https://www.jetify.com/docs/devbox) then:

```sh
devbox install
```

## Install Python packages

```sh
devbox run install_python_packages
```

## Install C++ kernel for JupyterLab

To support C++, we use [xeus-cling](https://github.com/jupyter-xeus/xeus-cling).
It's already installed as a [Nix](https://search.nixos.org/packages) package above.

To install its xeus-cling kernel to JupyterLab:

```sh
devbox run install_xeus_cling_kernel
```

## Start JupyterLab

```sh
devbox run jupyterlab
```
