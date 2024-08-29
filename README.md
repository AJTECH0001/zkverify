# Sending the Proof to zkVerify For Verification

## Prerequisite Reading
Before proceeding with the instructions on ```sending your proof to zkVerify for verification```, it is recommended to read the previous post that provides detailed context and background. This will ensure you have all the necessary knowledge and setup to successfully complete the process.

[Read the Previous Post on dev.io](https://dev.to/ajtech0001/developers-guide-zkverify-i3e)

This post covers:

Understanding Zero-Knowledge Proofs (ZKP)

Setting Up Your Development Environment

Generating and Converting Proof Files

Please make sure to go through this post thoroughly before continuing with the steps below.

## Send the proof to zkVerify

Firstly, head over to this link -  https://polkadot.js.org/apps/?rpc=wss%3A%2F%2Ftestnet-rpc.zkverify.io#/extrinsics

Once you are there, you will be asked to connect to the wallet. After you are connected, you will see a screen like below. Then, select your account from the option provided.

![Screen Shot 2024-08-29 at 10 09 17 AM](https://github.com/user-attachments/assets/495ab8b3-32b5-4fef-add5-51c15dd3b6d0)

Next, you need to choose ```settlementGroth16Pallet``` and ```submitProof``` which are like so:

![Screen Shot 2024-08-29 at 10 15 22 AM](https://github.com/user-attachments/assets/1d9ef2de-ffce-4b18-9d6b-3322cd5d5add)

Now, in the ```vkOrHash``` section, choose ```Vk``` instead of Hash.

![Screen Shot 2024-08-29 at 10 26 16 AM](https://github.com/user-attachments/assets/ad854237-ad04-4568-b885-c43c5231f031)

Next, we will need to return to the JSON files we generated during the previous lesson. First, let’s go to the ```verification_key_zkv.json``` file and paste the fields from that file. Make sure that you do not include the quotes.

![Screen Shot 2024-08-29 at 10 36 38 AM](https://github.com/user-attachments/assets/fca4b2eb-bd73-485d-8a5d-3b7b09b8e62f)

For ```gammaAbcG1```, we need to add an item as we have two fields by pressing on ‘Add item’ and then adding both of them like below.

![Screen Shot 2024-08-29 at 10 41 48 AM](https://github.com/user-attachments/assets/8fe1f61d-b37f-43f7-ae00-8e4aa82e6f7b)

The next step is to go to the file ```proof_zkv.json``` and paste copy ```a```, ```b```, and ```c``` inputs from the file and paste them in the respective fields like so:

![Screen Shot 2024-08-29 at 10 51 20 AM](https://github.com/user-attachments/assets/1fbd5643-1345-4daf-8651-af862e02f666)

The last and final step is to go to public_zkv.json file and copy and paste in the last field. Now our final stage of submission before submitting the transaction looks like below:

![ultraplonk-proof](https://github.com/user-attachments/assets/6be39d74-0d13-4dbc-b839-bd6846e5504f)

## Submit the transactions

### The final stage is to now submit the transaction.

Click on the ‘Submit transaction’ button and you will see a page where you can sign and submit the transaction.

![001](https://github.com/user-attachments/assets/16cf170d-1f9b-4652-8957-fc6402e51f14)

You now need to ‘Approve’ the transaction with your Talisman wallet. After you approve the transaction, wait for a few seconds as your transaction is getting completed. Once your transaction is completed, you will get a notification from Talisman wallet.

![002](https://github.com/user-attachments/assets/0e08a128-0fc4-4978-b1c3-482bb2838d06)

Now that your transaction is complete, copy your Talisman wallet address and paste it into the explorer - https://testnet-explorer.zkverify.io/v0

![Screen Shot 2024-08-29 at 2 36 19 PM](https://github.com/user-attachments/assets/bc755419-fc96-412a-b338-9db8ea169839)

Now if you click on your Extrinsic ID, you can see your transaction here:

![Screen Shot 2024-08-29 at 2 38 54 PM](https://github.com/user-attachments/assets/ba90b996-1c71-4c3c-b0bd-5feb7928b119)

Learn: Dive into the detailed zkVerify documentation https://docs.zkverify.io/.





