# Multithread Ethereum Bruteforce
Ethereum Bruteforce Node.js script that uses the cluster module to create multiple worker processes to generate random Ethereum keypairs and check if the public address corresponding to the private key is in a Set of full addresses from data.txt. If a match is found, private key and address will be saved inside match.txt

## Installation

1. Install Node.js on your system.
2. Clone this repository or download the script.
3. Open a terminal or command prompt and navigate to the directory where the script is located.
4. Run npm install to install the required dependencies.

## For people without technical experience you can buy the compiled application for windows from here:
[https://www.buymeacoffee.com/CorvusCodex/e/142988](https://www.buymeacoffee.com/CorvusCodex/e/147806?from_page=home)

Keep in mind that a Windows app won’t speed up searching or guarantee success.

<h3 align="left">Support:</h3>
<p><a href="https://www.buymeacoffee.com/corvuscodex"> <img align="left" src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" height="50" width="210" alt="corvuscodex" /></a></p><br><br>

<br><br>
Or donate:
BTC: bc1q7wth254atug2p4v9j3krk9kauc0ehys2u8tgg3  <br><br>
ETH & BNB: 0x68B6D33Ad1A3e0aFaDA60d6ADf8594601BE492F0

## Usage

1. Edit file data.txt in the same directory as the script and add the Ethereum addresses you want to search for, one per line start with 0x. (Like 3 exmples included). Make sure there is nothing(new line,spaces, etc...) after last address.
2. Run node app.js to start the script.
3. Chose display version, default is 1
4. The script will display the loop count and keys generated per minute for each worker process.
5. The Script look for a FULL address from data.txt
6. If a match is found, the script will save the wallet and its private key (seed) to a file named match.txt and exit.

## Dependencies
This script uses the following dependencies:

1. cluster: Node.js module to create multiple worker processes
2. fs: Node.js module to read and write files
3. os: Node.js module to get system information
4. blessed: A library for creating terminal-based user interfaces
5. ethers: A library for interacting with the Ethereum blockchain

## Check out Bitcoin Brute-Force Project
https://github.com/CorvusCodex/Multithread-Bitcoin-Brute-Force

## Disclaimer

The code within this repository comes with no guarantee, the use of this code is your responsibility. I take NO responsibility and/or liability for how you choose to use any of the source code available here. By using any of the files available in this repository, you understand that you are AGREEING TO USE AT YOUR OWN RISK. Once again, ALL files available here are for EDUCATION and/or RESEARCH purposes ONLY. The chances of finding a match are extremely low and it is not recommended to use this script for any illegal or unethical activities.


MIT License

Copyright (c) 2023 CorvusCodex

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
