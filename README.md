RISC-0 Receipt Verifier
----------------------

This is a python implementation of a verifier for the [RISC-0](https://www.risczero.com/) Receipt. 

Much of this code was cribbed directly from the [Rust RISC-0 repo](https://github.com/risc0/risc0), Thanks RISC-0 Team!

*WARNING:* This was written for a hackathon, it has not been audited for security.



## Usage



```sh
(.venv) ben@Algo-Guidarelli:~/py-risc0$ python main.py -h
usage: Risc0 Verifier [-h] [--path PATH] [-name NAME]

Verifies a Risc0 execution receipt

options:
  -h, --help            show this help message and exit
  --path PATH, -p PATH  Path to the execution artifacts
  -name NAME, -n NAME   Name of the program
```

*NOTE:* I've only tried this on one trivial program, the source is included in the `./programs` directory



### TODO:

- document/add comments to explain what is happening
- testing
- standardize encoding/decoding, lots of `to_elem` or `{encode|decode}_mont` in weird spots
- allow other `EXT_SIZE` options
