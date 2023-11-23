Quantum Circuit for Bernstein-Vazirani Algorithm

In this quantum circuit, we implement the Bernstein-Vazirani algorithm to find the hidden binary string sn. The algorithm efficiently determines the hidden string using a single query to the oracle function.

Quantum Circuit Description

Initialization:
A quantum circuit is created with n+1 qubits and n classical bits.
Hadamard gates are applied to all qubits except the last one.
A barrier is added for clarity.

Oracle Application:
A Pauli-X gate is applied to the last qubit.
A Hadamard gate is applied to the last qubit.
Using a for loop, controlled-X (CNOT) gates are applied based on the positions of '1' in the binary string sn. This simulates the application of the oracle function.
Another barrier is added for clarity.

Hadamard Transformation:
Hadamard gates are applied to all qubits.
Another barrier is added for clarity.

Measurement:
Measurements are performed on all qubits.
The histogram visualizes the outcome of the quantum measurement.

Simulation Results:
Running the circuit on a quantum simulator yields that the hidden binary string sn is '101'. The histogram visualizes the outcome of the quantum measurement.

