Open-Wallet-Format
==================
Bitcoin Wallet Convertor


OWF.py reads the keys from Bitcoin-QT wallet (e.g wallet.dat) and exports them to MultiBit wallet format (e.g multibit.key) but also applicable for Blockchain.info imports


Why should I use this?
---------------------
To Convert your wallet.dat (or exported wallet from Bitcoin-QT) to:
** MultiBit Wallet
** Blockchain Importable format
** Backup your private keys in a format that would not be as complicated as wallet.dat and less possible to be corrupted

WARNING: the output is not encrypted so take good care of the file! 


Usage:
-------
Usage: OWF.py [options]

Options:
  --version             show program's version number and exit
  -h, --help            show this help message and exit
  --wallet=WALLET       wallet.dat or the exported wallet from Bitcoin-QT to
                        be converted
  --newwallet=NWWALLET  New wallet name (multibit format) (in the
                        same directory as the --wallet

Example
-------
./OWF.py --wallet ./wallet.dat
./OWF.py --wallet ./wallet.dat ./newwallet.key



I used jackjack-jj fork of Pywallet.py (https://github.com/jackjack-jj/pywallet) to read wallet.dat and it is included in this repository.
