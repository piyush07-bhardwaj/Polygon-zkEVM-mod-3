# Poly-zkEVM-mod-3

Poly-zkEVM-Circuit is a project that implements polynomial zero-knowledge succinct non-interactive arguments of knowledge (Poly-zkSNARK) for circuits. It allows you to generate and verify zero-knowledge proofs for the correctness of computations performed by circuits.

## Description

This project implements a logical gate circuit using the circom programming language. The circuit implements the following truth table:

```
A B X Y Q
0 0 0 1 1
0 1 0 0 0
1 0 0 1 1
1 1 1 0 1
```

The goal of the project is to prove that you know the inputs A=0 and B=1 that yield a 0 output. 

### Prerequisites

To run Poly-zkSNARK-Circuit, you need to have the following installed on your system:

- Node.js (https://nodejs.org) - JavaScript runtime environment
- npm (Node Package Manager, comes with Node.js installation)


### Installing

1. Clone the repository:

   ```bash
   https://github.com/piyush07-bhardwaj/Polygon-zkEVM-mod-3
   
   
2. Install the required dependencies :

   ```bash
    cargo build --release
    cargo install --path circom
   
3. Installing snarkjs :

   ```bash
   npm install -g snarkjs


## Usage

To generate and verify zero-knowledge proofs for your circuits, follow these steps:

1. Define your circuit in the `circuits` folder.

2. Create an input JSON file in the `Proof` folder, specifying the inputs to your circuit.

3. Run the `genProof.js` script:

`node genProof.js`

This will compile our circuit, calculate the witness, and generate the proof and public signals.


## Contributing

Contributions to Poly-zkEVM-Circuit are welcome! If you find any issues or want to add new features, feel free to open a pull request. 

## Author

Piyush Bhardwaj


