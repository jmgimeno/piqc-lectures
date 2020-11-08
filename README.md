# A Practical Introduction to Quantum Computing: from qubits to quantum machine learning and beyond

Organized by:

- CERN Quantum Technology Initiative
- CERN openlab

by Elias Fernandez-Combarro Alvarez (Universidad de Oviedo (ES)

## Links

- [Access to lectures](https://indico.cern.ch/event/970903/)
- [Quirk](https://algassert.com/quirk)
- [Quiskit](https://qiskit.org/)
- [IBM Quantum Experience](https://quantum-computing.ibm.com/)
- [Google Colab](https://colab.research.google.com/)

## Dockerized Qiskit-notebook

    docker pull sanori/qiskit-notebook

Qiskit-notebook is a Jupyter Docker Stack image for IBM Qiskit.

This image includes the visualization package.

### How to use

After executing the following command, connect to localhost:8888/?token=blahblah through the link in the text that comes out.

    docker run -it --rm -p 8888:8888 sanori/qiskit-notebook

You can save Jupyter notebooks in the current directory by attaching the current directory ($PWD) to work directory as follows:

    docker run -it --rm -p 8888:8888 -v "$PWD":/home/jovyan/work sanori/qiskit-notebook

# IBM QUantum Experience

Before using the IBMQ provider, we must register our account.

    IBMQ.delete_accounts() # only after generating new token
    IBMQ.save_account("<token>")

will do the trick.
