This Repository contains get started instruction how to use NEURON + NetPyNE. 
This README contains installation instruction. For more information check Wiki page on GitHub.

# Anaconda
Since some libs may have conflicting version with NetPyNE it's better to create a new env called neuron with Python 3.6

* `conda create --name neuron python=3.6`
* `conda activate neuron`

# NEURON

### Install NEURON

* Download `neuron.deb` from https://www.neuron.yale.edu/neuron/download
* `dpkg -i neuron.deb`
* add to ~/.bashrc: 
`export PYTHONPATH="$PYTHONPATH:/usr/local/nrn/lib/python/"`
* Test NEURON Python in console:
  * `python`
  * `from neuron import h, gui`
  * if you see that NEURON has started - it works fine

### Add Python NEURON to PyCharm

* Setting -> Project Interpreter -> click on interpreter list and select "Show All" -> Add or select your interpreter -> click "Show paths for the selected interpreter"
* add the path: /usr/local/nrn/lib/python

# NetPyNE
Install NetPyNE

* `pip install netpyne`
* `pip install netpyne-ui`

# Test all

* If you want to run it from IDE, preferably start IDE from the console to make sure PYTHONPATH is correctly loaded.
* Download:
  * http://netpyne.org/_downloads/25249eff85a9f9e5883f5bf9edd3950d/tut1.py 
  * https://raw.githubusercontent.com/Neurosim-lab/netpyne/master/examples/HHTut/HHTut.py
* save to the same folder
* run `tut1.py`

