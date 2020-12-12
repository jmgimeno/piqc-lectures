# A Practical Introduction to Quantum Computing: from qubits to quantum machine learning and beyond

Organized by:

- CERN Quantum Technology Initiative
- CERN openlab

by Elias Fernandez-Combarro Alvarez (Universidad de Oviedo (ES)

## Links

- [Access to lectures](https://indico.cern.ch/event/970903/)
- [Quirk](https://algassert.com/quirk)
- [Quiskit](https://qiskit.org/)
- [Installing Quiskit](https://qiskit.org/documentation/install.html)
- [IBM Quantum Experience](https://quantum-computing.ibm.com/)
- [Google Colab](https://colab.research.google.com/)
- [D-Wave's Leap](https://www.dwavesys.com/take-leap)
  - [MaxCut example with D-Leap](https://bit.ly/3dPos2L)
- [Sau Lan Wu - HEP Analysis at LHC w/ Quantum Machine Learning on Q. Computer Simulators & Q. Hardware](https://youtu.be/rwZrmSs2nO8)

## Recordings

- [Lecture 1](https://youtu.be/jwHM8AHOtJ0)
- [Lecture 2](https://youtu.be/SPQ-rvtaREs)
- [Lecture 3](https://youtu.be/wX_vmpbQGU4)
- [Lecture 4](https://youtu.be/a7L2m2qlEIw)
- [Lecture 5](https://youtu.be/LFewKe_tWME)
- [Lecture 6](https://youtu.be/I6xnxUSubD0)

## Dockerized Qiskit-notebook

    docker pull sanori/qiskit-notebook

Qiskit-notebook is a Jupyter Docker Stack image for IBM Qiskit.

This image includes the visualization package.

### How to use

After executing the following command, connect to localhost:8888/?token=blahblah through the link in the text that comes out.

    docker run -it --rm -p 8888:8888 sanori/qiskit-notebook

You can save Jupyter notebooks in the current directory by attaching the current directory ($PWD) to work directory as follows:

    docker run -it --rm -p 8888:8888 -v "$PWD":/home/jovyan/work sanori/qiskit-notebook

## IBM Quantum Experience

Before using the IBMQ provider, we must register our account.

    IBMQ.delete_account() # only after generating new token
    IBMQ.save_account("<token>")

will do the trick.
