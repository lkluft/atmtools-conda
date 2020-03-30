# Atmtools conda configuration

Configuration files to create conistent [Anaconda] environments.

The [condarc](condarc) controls the basic behavior of the `conda` command, like
changing the shell prompt or the list of channels to search for packages.
It is stored in the user's home directory:
```bash
cp condarc $HOME/.condarc
```

The [environment.yml](environment.yml) can be used to either create a new
environment or to update the existing base environment.
```bash
conda env create -f environment.yml  # new environment
conda env update -n base -f environment.yml  # update `base` environment
```

[Anaconda]: https://www.anaconda.com/distribution
