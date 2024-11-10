# QOSF-Mentorship-Program-Test-Selection
QOSF Mentorship Program Test/Selection Task Question 1 Solution

**Task 1 State Vector simulation of quantum circuits**

For this task, you will implement a state vector simulator for quantum circuits from scratch. The goal is to demystify how to simulate a quantum computer and to demonstrate your familiarity with quantum circuits.

1) Naive simulation using matrix multiplication

Remember that  [1, 0] = |0> is the most common representation of the single-qubit zero state, and analogously [0, 1] = |1>. 

Most matrix representations of quantum gates you can find online follow this convention. For example, the X gate can be written as

X = [〖_(1  0)^(0   1)〗]

Using the Kronecker product and the np.kron function in numpy (we are using it as an example, but you can use any library you want to), you can create a vector of length 2^n representing an n-qubit quantum state, and matrix representation of X, H, and CNOT gates. 

Hint: The single-qubit Identity matrix is

I = [〖_(0  1)^(1   0)〗]
 
Define a quantum circuit consisting of these gates and apply the gates sequentially to the state vector via matrix multiplication. 

Plot the runtime of your code as a function of the number of qubits. How many qubits can you simulate this way? 

