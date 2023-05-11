# Multithead Ethereum Bruteforce
Ethereum Bruteforce Node.js script that uses the cluster module to create multiple worker processes to generate random Ethereum keypairs and check if the public address corresponding to the private key is in a Set of addresses read from data.txt. If a match is found, private key and address will be saved inside match.txt

## Installation

1. Install Node.js on your system.
2. Clone this repository or download the script.
3. Open a terminal or command prompt and navigate to the directory where the script is located.
4. Run npm install to install the required dependencies.

## Usage

1. Create a file named data.txt in the same directory as the script and add the Ethereum addresses you want to search for, one per line.
2. Run node index.js to start the script.
3. The script will display the loop count and keys generated per minute for each worker process.
4. If a match is found, the script will save the wallet and its private key (seed) to a file named match.txt and exit.

## Dependencies
This script uses the following dependencies:

1. cluster: Node.js module to create multiple worker processes
2. fs: Node.js module to read and write files
3. os: Node.js module to get system information
4. blessed: A library for creating terminal-based user interfaces
5. ethers: A library for interacting with the Ethereum blockchain
