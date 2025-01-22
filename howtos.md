# HOW Tos

1. https://docs.quantum.ibm.com/guides/setup-channel#iqp

Execute the following in a trusted environment like an environment in your own computer.
```python
token = "<your-token>"
```
```python
from qiskit_ibm_runtime import QiskitRuntimeService
 
QiskitRuntimeService.save_account(
  token=token,
  channel="ibm_quantum" # `channel` distinguishes between different account types
)
```

2. Installing Qiskit: https://docs.quantum.ibm.com/guides/install-qiskit
Following are some useful things that you would like to install.
First of all create a python environment. Then install the following packages through PyPI.
```shell
pip install qiskit
pip install qiskit-ibm-runtime
pip install qiskit[visualization]
pip install jupyter
```

In zsh terminal use quotes for the visualization package.
```shell
pip install 'qiskit[visualization]'
```