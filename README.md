jk_pypi
==========

Introduction
------------

This python module allows retrieving data from pypi.org. Please note that currently it has very limited capabilities.

Information about this module can be found here:

* [github.org](https://github.com/jkpubsrc/python-module-jk-pypi)
* [pypi.python.org](https://pypi.python.org/pypi/jk_pypi)

How to use this module
----------------------

### Import this module

Please include this module into your application using the following code:

```python
import jk_pypi
```

### Instantiate main class

For getting access to the PyPi server instantiate `PyPi`:

```python
pypi = jk_pypi.PyPi()
```

This object will now contact `pypi.org` for you and retrieve information. By default requests to `pypi.org` will be cached internally
in this object to reduce load on the `pypi.org` server.

### Retrieve the version of a module

Here is an example about how to get latest version information about a module:

```python
v = pypi.getModuleVersion("jk-pypi")
print(v)
```

If the module is not found `None` is returned.

### Retrieve the download URL of a module

You can also retrieve the download URL of a module:

```python
v = pypi.getDownloadURL("jk-pypi")
print(v)
```

This is useful for offline installation.

Contact Information
-------------------

This is Open Source code. That not only gives you the possibility of freely using this code it also
allows you to contribute. Feel free to contact the author(s) of this software listed below, either
for comments, collaboration requests, suggestions for improvement or reporting bugs:

* Jürgen Knauth: jknauth@uni-goettingen.de, pubsrc@binary-overflow.de

License
-------

This software is provided under the following license:

* Apache Software License 2.0



