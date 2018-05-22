bash <( curl https://raw.githubusercontent.com/demesm/Aegeus/master/aegeus_install.sh )


***Step 8***
* Paste the code below into the Bitvise terminal then press enter

`bash aegeus_install.sh`

![Example-Bash](https://i.imgur.com/myvmKTE.png)

***

***Step 9***
* Sit back and wait for the install (this will take 10-20 mins)
***

***Step 10***
* When prompted to enter your Masternode Gen key - press enter

![Example-installing](https://i.imgur.com/sLvWd1S.png)
***

***Step 11***
* You will now see all of the relavant information for your server.
* Keep this terminal open as we will need the info for the wallet setup.
![Example-installing](https://i.imgur.com/Q87LcnW.png)
***

## Section D: Preparing the Local wallet

***Step 1***
* Download and install the Aegeus wallet [here](https://github.com/AegeusCoin/aegeus/releases)
***

***Step 2***
* Send EXACLY 5,000 Aegeus to a receive address within your wallet.
***

***Step 3***
* Create a text document to temporarily store information that you will need. 
***

***step 4***
* Go to the console within the wallet 

![Example-console](https://i.imgur.com/6NM7G9a.png)
***

***Step 5***
* Type the command below and press enter 

`masternode outputs` 

![Example-outputs](https://i.imgur.com/GD7Ro1m.png)
***

***Step 6***
* Copy the long key (this is your transaction ID) and the 1 or 2 at the end (this is your output index)
* Paste these into the text document you created earlier as you will need them in the next step.
***

# Section E: Connecting & Starting the masternode 

***Step 1***
* Go to the tools tab within the wallet and click open "masternode configuration file" 
![Example-create](https://i.imgur.com/COsfvfA.png)
***

***Step 2***

* Fill in the form. 
* For `Alias` type something like "MN01" **don't use spaces**
* The `Address` is the IP and port of your server (this will be in the Bitvise terminal that you still have open).
* The `GenKey` is your masternode GEN key (This is also in the Bitvise terminal that you have open).
* The `TxHash` is the transaction ID/long key that you copied to the text file.
* The `Output Index` is the 0 or 1 that you copied to your text file.
![Example-create](https://i.imgur.com/9b1I3bk.png)

Click "File Save"
***

***Step 3***
* Close out of the wallet and reopen Wallet
*Click on the Masternodes tab "My masternodes"
* Click start all in the masternodes tab
***

***step 4***
* Check the status of your masternode within the VPS by using the command below:

`aegeus-cli masternode status`

*You should see ***status 9***

If you do, congratulations! You have now setup a masternode. If you do not, please contact support and they will assist you.
