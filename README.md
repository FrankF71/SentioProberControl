[![GitHub issues](https://img.shields.io/github/issues/SentioProberDev/SentioProberControl.svg?maxAge=360)](https://github.com/SentioProberDev/SentioProberControl/issues)
[![Version](https://img.shields.io/github/release/SentioProberDev/SentioProberControl.svg?maxAge=360)](https://github.com/SentioProberDev/SentioProberControl/releases/)
[![Github All Releases](https://img.shields.io/github/downloads/SentioProberDev/SentioProberControl/total.svg)](https://github.com/SentioProberDev/SentioProberControl/releases/)
# SENTIO® Prober Control - Python Bindings
This archive contains a package with python bindings to control a [MPI SENTIO® probe station](https://www.mpi-corporation.com/ast/engineering-probe-systems/mpi-sentio-software-suite/).

![](https://www.mpi-corporation.com/wp-content/uploads/2019/12/1.-TS3500-SE-with-WaferWallet_frontview.jpg)

## Instructions for installing the SENTIO® prober control Python package

1.) Download the latest python package from:

https://github.com/SentioProberDev/SentioProberControl/releases

2.) Install the python package with pip:

```python -m pip install --user sentio-prober-control-3.5.0.tar.gz```

Please note that pip will automatically uninstall an older version of the sentio_prober_control repository, if one is found.

## Troubleshooting

If you have problems getting the package to work. Check wether an old version of the sentio-prober-control is still installed. To do so type

```python -m pip list```

if an older version is listed uninstall it first by using the command. 

```python -m pip uninstall sentio-prober-control```

After the uninstallation you can proceed with the installation as explained in the section above.

## Instructions for package maintainer (updating the package) 

*The following instructions are for creating a new release of the package. If you only want to use the package you do not need to do this! Just follow the instructions listed above for installing an existing package.*

1.) Get the latest version of setuptools and wheel:

```python -m pip install --user --upgrade setuptools wheel```

2.) create the distribution archive:

cd into the archive (where setup.py) is located.

```python setup.py sdist bdist_wheel```

This command will create the dist folder.

```
dist/
  sentio-prober-control-3.5.0-py3-none-any.whl
  sentio-prober-control-3.5.0.tar.gz
```

3.) Create a new release on GitHub with the new binary archive
