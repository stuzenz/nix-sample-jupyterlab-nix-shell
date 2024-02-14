# Context for this project

This project was to help out a redditor build a working jupyterlab environment as per here

https://www.reddit.com/r/NixOS/comments/1aq58xv/jupyter_and_python_on_nixos/

This is not too hard to do - but there is some layered considerations:

1.  Shall we do it using a simple nix-shell project configuration or nix develop flake or a 3rd party abstraction like devenv?
    
2.  What shall I do from nix packaging and what shall I do from a python virtual environment or conda environment (virtual environment is the one we will use here)
    
3.  For my python venv (virtual environment) am I going to get my nix instantiation to run a requirements.txt file to install other python packages that are not in the nixos system packages repo?
    
4.  Am I going to use the browser for jupyterlab or us vs code with jupyter lab (if the latter you will need some of the vs code extensions installed)
    

The above is really just written to get you to get start contextualising what is happening.

I have created a public repo here for you. I haven't fully customised it or removed things I have in it - but it has numpy as an example

`git clone` the repo, `cd` into the project directory, run `nix-shell`, that will instantiate the project environment, then run `jupyter-lab` and follow the instructions

[https://github.com/stuzenz/nix-sample-jupyterlab-nix-shell/tree/main](https://github.com/stuzenz/nix-sample-jupyterlab-nix-shell/tree/main)
