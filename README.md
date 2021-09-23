# Unit-18: Proof of Authority Development Chain

Summary: 
<br>
This project is designed as a manual for the creation of a testnet for a fictitious bank. The following guide uses visuals in accordance with the framework set out in the assignment instructions. The password for each account has been provided to the central grader. 

Before you start:
<br>
You will need to create a new directory for your new network. You can all it anything you want. You will then have to create a 'screenshots' subfolder as well.
<p>
  
Step 1

<br>
<p align="center"><img src="https://github.com/ThomasJScott3/unit-18-blockchain/blob/main/Screenshots/Step%201.PNG"></img></p>
<br>
Next, you will have to open geth. Then you need to create accounts for at least two nodes for your network. Bear in mind that each node will require a separate datadir for each one in geth. Follow the commands shown in the screenshot above to do this.
<p>

 Step 2

<br>
<p align="center"><img src="https://github.com/ThomasJScott3/unit-18-blockchain/blob/main/Screenshots/Step%202.PNG"></img></p>
<br>
Next, you will need to run puppeth. Then name your network, and then select the option to 'configure a new genesis' block (a.k.a option 2). Follow the steps outlined in the screenshot above for the creation of said block.
<p>

Step 3

<br>
<p align="center"><img src="https://github.com/ThomasJScott3/unit-18-blockchain/blob/main/Screenshots/Step%203.PNG"></img></p>
<br>
For the next step, please choose the 'Clique (Proof of Authority)' consensus algorithm option. After that, paste both account addresses from the first step one at a time into the list of accounts to seal. Follow the remaining steps shown in the screenshot to continue.
<p>

Step 4

<br>
<p align="center"><img src="https://github.com/ThomasJScott3/unit-18-blockchain/blob/main/Screenshots/Step%204.PNG"></img></p>
<br>
Next, you will need to complete the rest of the prompts shown above. When you return to the main menu, please choose the 'Manage existing genesis' option. From there, please select 'export genesis configurations.' This action will fail in creating two of the files. However, you only need networkname.json.
<p>

Step 5

<br>
<p align="center"><img src="https://github.com/ThomasJScott3/unit-18-blockchain/blob/main/Screenshots/Step%205.PNG"></img></p>
<br>
Per the screenshot above, you can delete the file called 'yournetworkname-harmony.json.'
<p>

Step 8

<br>
<p align="center"><img src="https://github.com/ThomasJScott3/unit-18-blockchain/blob/main/Screenshots/Step%208.PNG"></img></p>
<br>
Per the screenshot above, input the following command: 'geth --datadir node1 --unlock "YOUR ACCOUNT ADDRESS FOR NODE 1" --mine --rpc --allow-insecure-unlock'
<p>

Step 9

<br>
<p align="center"><img src="https://github.com/ThomasJScott3/unit-18-blockchain/blob/main/Screenshots/Step%2019.PNG"></img></p>
<br>
Per the screenshot above, input the following command: 'geth --datadir node2 --unlock "YOUR ACCOUNT ADDRESS FOR NODE 2" --mine --port 30304 --bootnodes "enode://YOUR_NODE_1_ENODE_ADDRESS@127.0.0.1:30303" --ipcdisable --allow-insecure-unlock' Be sure to get the enode address from the geth window for the first node.
<p>

Step 10

<br>
<p align="center"><img src="https://github.com/ThomasJScott3/unit-18-blockchain/blob/main/Screenshots/Step%2010.PNG"></img></p>
<br>
If the operation is successful, you should see the following in each window. This signifies that mining is taking place.
<p>

Step 11
<br>
<p align="center"><img src="https://github.com/ThomasJScott3/unit-18-blockchain/blob/main/Screenshots/Step%2011.PNG"></img></p>
<br>
Next, you will need to open up MyCrypto and open up the keystore wallet for your first account. THe password for my nodes have been provided to the central grader.
<p>

Step 12
<br>
<p align="center"><img src="https://github.com/ThomasJScott3/unit-18-blockchain/blob/main/Screenshots/Step%2012.PNG"></img></p>
<br>
Next, you will send a transaction from your first account to the second one. Make sure to have both addresses queued up for easy access.
<p>

Step 13
<br>
<p align="center"><img src="https://github.com/ThomasJScott3/unit-18-blockchain/blob/main/Screenshots/Step%2013.PNG"></img></p>
<br>
Next, you will be asked to confirm the transaction and send it. Click 'send' to proceed.
<p>

Step 14
<br>
<p align="center"><img src="https://github.com/ThomasJScott3/unit-18-blockchain/blob/main/Screenshots/Step%2014.PNG"></img></p>
<br>
You should see the following green pop-up in MyCrypto if the transaction was successfully sent.
<p>

Step 15
<br>
<p align="center"><img src="https://github.com/ThomasJScott3/unit-18-blockchain/blob/main/Screenshots/Step%2015.PNG"></img></p>
<br>
Next, go back to your geth windows. You should see the following activity indicating that your testnet nodes are processing the transaction.
<p>

Step 16
<br>
<p align="center"><img src="https://github.com/ThomasJScott3/unit-18-blockchain/blob/main/Screenshots/Step%2020.PNG"></img></p>
<br>
If the action was successful, you should be able to see the following screen when you go to the transaction verification screen in MyCrypto.
<p>

Step 17
<br>
<p align="center"><img src="https://github.com/ThomasJScott3/unit-18-blockchain/blob/main/Screenshots/Step%2021.PNG"></img></p>
<br>
Be sure to test your testnet with multiple transactions. For example, how does cranking up the gas fee impact the speed of the transaction?
<p>

Step 18
<br>
<p align="center"><img src="https://github.com/ThomasJScott3/unit-18-blockchain/blob/main/Screenshots/Step%2022.PNG"></img></p>
<br>
For extra credit, open your second account's keystore wallet and send the majority of the test ETH to the first account.
<p>

Step 19
<br>
<p align="center"><img src="https://github.com/ThomasJScott3/unit-18-blockchain/blob/main/Screenshots/Step%2023.PNG"></img></p>
<br>
Next, refresh your second account's wallet. You should have very little ETH left if the operation was successful.
<p>

Step 20
<br>
<p align="center"><img src="https://github.com/ThomasJScott3/unit-18-blockchain/blob/main/Screenshots/Step%2024.PNG"></img></p>
<br>
Now go to your first account. As you can see, you have almost double the test ETH! Pat yourself on the back, because you have just executed a multinodal transaction. You have sent test ETH one way and then sent even more back the other way!
<p>
## End of Manual


