# Qiskit-Aer

This is a working draft for the Qiskit-Aer simulator framework for Qiskit-Terra. This is the development repository and has no guarantee of stability or correctness.


## Repository contents

* The  **aer** folder contains the Qiskit-Aer python module for use with Qiskit-Terra.
* The **cmake** folder contains cmake scripts for building the simulator
* The **src** folder contains the C++ source files for building the simulator.
* The **examples** folder contains example qobj files for the simulator.
* The **standalone** folder contains a stand-alone executable that can be used for development and testing. Note that stand-alone building will be removed before release and will not be supported.
* The **test** folder contains simulator unit tests.

## Documentation

See the [Qiskit Aer wiki](https://github.ibm.com/IBMQuantum/qiskit-aer/wiki) for documentation.


## Installation

Follow these steps for installing Terra simulator addons:

```bash
qiskit-aer$ cd aer/qv_addon
qiskit-aer/aer/qv_addon$ python ./setup.py bdist_wheel
```

Once the build finishes, we just need to install the wheel package in our
prefered python virtual environment:

```bash
qiskit-aer/aer/qv_addon$ cd dist
qiskit-aer/aer/qv_addon/dist$ pip install qiskit_addon_qv-0.0.0-cp36-cp36m-linux_x86_64.whl
```

We are all set! Now we ready to start using the simulator in our python code:
```python
from qiskit_addon_qv import AerQvSimulator

simulator = AerQvSimulator()
```
