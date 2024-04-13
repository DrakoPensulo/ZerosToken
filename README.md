# ZerosToken
ZerosToken Chia Asset Token

THIS TAIL IS PROVIDED AS IS WITH NO WARRANTY. IT HAS NOT BEEN AUDITED OR TESTED. FOR EDUCATIONAL PURPOSES ONLY. 
USE IT ON YOUR OWN RISK. YOU MAY LOSS SOME OF ALL OF YOUR ASSETS.

Asset ID 00000000024e1fb9fc47c7ec72854c6a987c4cc99f6535a4caca6154220eeda5

Intended behavior
      Everyone can mint any number of tokens ONLY BEFORE the block 6100281 (approximately Nov 03, 2024). NO MINTIG POSSIBLE AFTER THAT BLOCK. 
      Melting possible FOREVER AFTER the block 7771033 (approximately Oct 18, 2025) [NOT TESTED].

# How to mint

1) Install Chia Blockchain https://www.chia.net/downloads/
2) Install Python (if it has not been installed yet) https://www.python.org/
3) Install Git (if it has not been installed yet) https://git-scm.com/download/
4) Install the official CAT-minting-tool https://github.com/Chia-Network/CAT-admin-tool
5) In the Python venv enviroment execute the following command to mint 1 million Zeros... 0000 token (with fee 1m mojos). Total cost 0.001001 XCH.

cats --amount 1000000000 --fee 10000000 --send-to xch1___YOUR___ADDRESS___HERE_ --tail 'ff02ffff01ff02ffff03ff2fffff01ff02ffff03ffff22ff0bffff09ffff11ff80ff2f80ff81bd8080ffff01ff04ffff04ff0cffff04ff0aff808080ff8080ffff01ff08ffff018c4472616b6f50656e73756c6f8080ff0180ffff01ff04ffff04ff08ffff04ff0eff808080ff808080ff0180ffff04ffff01ffff5753ff83769399835d1539ff018080' --solution '()'

# Testnet Zeros... T0000 token

Asset ID 0000000062fccdc5df5dc44770a614f85154c27298e22bdcedbcb76af5056e5c

Testnet version of the Zeros... 0000 token should be mintable and meltable up to year 2101. 


1) - 4) as above
5) Change network to Testnet11 via chia configure -t true
6) To mint 1m Testnet Zeros... T0000 token execute (total cost 0.001001 TXCH)
cats --amount 1000000000 --fee 1000000 --send-to txch1___YOUR___ADDRESS___HERE_ --tail 'ff02ffff01ff02ffff03ff2fffff01ff02ffff03ffff22ff0bffff09ffff11ff80ff2f80ff81bd8080ffff01ff04ffff04ff0cffff04ff0aff808080ff8080ffff01ff08ffff018c4472616b6f50656e73756c6f8080ff0180ffff01ff04ffff04ff08ffff04ff0eff808080ff808080ff0180ffff04ffff01ffff5753ff8304ef818407bfab2dff018080' --solution '()'

7) Melting is possible via the forked CAT-minting-tool from https://github.com/DrakoPensulo/CAT-admin-tool  
To melt 1m Testnet Zeros... T0000 token execute, total cost 1m mojos, 0.001 TXCH should appear on your wallet and 1m Testnet Zeros... T0000 token should disappear.

cats --amount -1000000000 --fee 1000000 --send-to txch1___YOUR___ADDRESS___HERE_ --tail 'ff02ffff01ff02ffff03ff2fffff01ff02ffff03ffff22ff0bffff09ffff11ff80ff2f80ff81bd8080ffff01ff04ffff04ff0cffff04ff0aff808080ff8080ffff01ff08ffff018c4472616b6f50656e73756c6f8080ff0180ffff01ff04ffff04ff08ffff04ff0eff808080ff808080ff0180ffff04ffff01ffff5753ff8304ef818407bfab2dff018080' --solution '()'


CAT = Chia Asset Token https://chialisp.com/cats
TAIL = Token and Asset Issuance Limitations https://chialisp.com/cats/#tail


A bug reported: https://github.com/Chia-Network/chia-blockchain/issues/17727