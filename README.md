# **Error Correction with the Shor Code**
---

## **Introduction** 
This project extends your work in Week 21 to implement, simulate, and analyze the first ever error correction code proposed that can handle *any* single qubit errors (bit-flips, phase-flips, or others) using the Shor code (Sho95).

<br>

## **Description**
The Shor code is a natural extension of the Bit- and Phase- flip codes that avoid syndrome measurements where:

* A **bit-flip error** means $|0\rangle$ unintentionally turning into $|1\rangle$ or vice versa.
* A **phase-flip error** means $|+\rangle$ unintentionally turning into $|-\rangle$ or vice versa.

This code can be viewed as two levels of quantum error correction where:
1. The logical qubits are first encoded into a 3-qubit phase-flip code.
1. Each of the resulting physical qubits are encoded into a 3-qubit bit-flip code.

<br>

## **Key Questions**
In this project, you will answer the following questions:
1. How does using the Shor code compare to using no error correction? Are there any trends you notice?

1. When using the Shor code, how does the average fidelity change with increasing probability of errors? Why is this?

1. Are there any unexpected patterns in the average fidelity? Why do you think they might be happening if so?

<br>

## **Structure**
This project is broken into 3 parts:
> **Part 1**: Defining the Components
>
>> **Part 1.1**: The Phase-Flip Code
>>
>> **Part 1.2**: The Bit-Flip Code
>
> **Part 2**: Implementing the Shor Code
>
> **Part 3**: Analyzing the Shor Code
>
> **Wrapping Up**

<br>

## **Resources**
* [Week 21 Lab Solutions (Bit-Flip Code and Noise Models)](https://drive.google.com/file/d/1nbNfFwUp4eefAR95AG5q_nKSNAMgLmsc/view?usp=share_link)
* [Week 21 Homework Solutions (Phase-Flip Code)](https://colab.research.google.com/drive/1BYZrbBJKTtCCm11Z7No6rNN114fgllhU?usp=sharing)
* [Qiskit's `circuit.compose(...)` function documentation](https://qiskit.org/documentation/stubs/qiskit.circuit.QuantumCircuit.compose.html)
* [Qiskit's `Statevector(...)` documentation](https://qiskit.org/documentation/stubs/qiskit.quantum_info.Statevector.html)
* [Quantum Error Correction for Beginners](https://arxiv.org/pdf/0905.2794.pdf)
* [Scheme for reducing decoherence in quantum computer memory](https://journals.aps.org/pra/abstract/10.1103/PhysRevA.52.R2493): The original paper from by Shor proposing this code (behind a paywall)

---
