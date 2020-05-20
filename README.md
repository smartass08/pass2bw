# pass2bw

Utility to export a [pass password store](https://www.passwordstore.org/) to [BitWarden](https://bitwarden.com/).

## Requirements

This is a Python script with requirements specified in the `requirements.txt` file.

If you want to directly import the exported store on the command line, install the [BitWarden CLI](https://bitwarden.com/help/article/cli/).
Otherwise just use the online interface.

## Usage

To decrypt the password store, simply execute:
```bash
$ ./pass2bw --out=store.csv
```
Then inspect the `store.csv` to check that the export was successful.
If yes, import the store into BitWarden either online or with the CLI: 
```bash
$ bw import bitwardencsv store.csv
```
