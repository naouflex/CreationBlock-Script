# Find Contract Deployment Block

This Python script is designed to search for the block in which a smart contract was deployed on the Ethereum blockchain. The script uses the `web3` library to interact with the blockchain and search for the contract in a specified range of blocks. The search can be performed by a single thread or multiple threads or processes to improve performance.

## Prerequisites

To run this script, you will need the following:

- Python 3.7 or later installed
- `web3` library installed (`pip install web3`)
- `tqdm` library installed (`pip install tqdm`)
- `argparse` library installed (`pip install argparse`)
- `dotenv` library installed (`pip install python-dotenv`)

## Usage

To run the script, open a terminal window and navigate to the directory containing the script. Then run the following command:

`python find_contract_block.py <contract_address> [-s <start_block>]`


Where `<contract_address>` is the address of the contract you want to search for, and `-s` or `--start_block` (optional) is the block number to start scanning from (default: 0).

## Output

If the contract is found, the script will output the block number in which it was deployed. If the contract is not found, the script will output "Contract not found in any block". 

During the search, a progress bar will be displayed showing the percentage of blocks searched so far. 

## License

This script is licensed under the MIT License.
