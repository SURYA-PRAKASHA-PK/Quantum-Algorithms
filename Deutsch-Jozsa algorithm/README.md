Deutsch-Jozsa Algorithm

The Deutsch-Jozsa algorithm is a quantum computing algorithm that solves a specific type of problem faster than classical algorithms. The problem involves determining whether a given binary function is constant or balanced.

Oracle Construction:
Two types of oracles are constructed for the algorithm:

Constant Oracle (const_oracle):
The oracle flips the last qubit based on a randomly chosen constant value (0 or 1).
The constant value is stored in the variable output.

Balanced Oracle (balanced_oracle):
The oracle flips the last qubit if the corresponding bit in the binary string b_str is '1'.
The binary string b_str is set to "101" in this example.

Deutsch-Jozsa Circuit:
The quantum circuit for the Deutsch-Jozsa algorithm is constructed as follows:

Initialization:
Hadamard gates are applied to the first n qubits.
The last qubit is set to the state |1⟩ using X gate and then a Hadamard gate is applied.
A barrier is added for clarity.

Oracle Application:
The balanced oracle is applied to the circuit.
Another barrier is added for clarity.

Hadamard Transformation:
Hadamard gates are applied to the first n qubits.
Another barrier is added for clarity.

Measurement:
Measurements are performed on the first n qubits.
The histogram visualizes the outcome of the quantum measurement.

Simulation Results:
Running the circuit on a quantum simulator provides a histogram of measurement outcomes. In this example, the histogram should show a result other than all zeros if the oracle is balanced.


