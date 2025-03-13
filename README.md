# urToken (Function wise functionality is described in Code)

Description of working of Smart Contract is as follows:

## Functionalities

- Decentralized Protection of Native Tokens
- Decentralized Unprotection of Native Tokens
- Transfer urTokens (ultra resistant Tokens)
- Fee Collection System (Benefaction-fee)
- Award System
- Whitelist Mechanism
- Sign Key to Perform User Operations (Transactions)
- Master Key as Recovery Mechanism
- Quantum Resistant Approach

### Decentralized Protection of Native Tokens

**_Definition:_** On one side of the coin, it is an independent onchain 2FA (with extra functionalities). The main objective is to help prevent (and stop in full) crypto theft caused by bad actors infesting the ecosystem with constant phishing attacks, wallet drainers and other sophisticated exploits (see Bybit hack). The scope of the protection includes *potential quantum threats* (prevented by incorporating Dilithium-Crystals into the security scheme).

It works by abstracting away the wallet's private keys to sign transactions and allowing the user to set their own (A) Classical Sign Key or (B) Quantum Resistant Sign Key (optional).

On the other side of the coin, it is a mechanism design in wich, without having a centralized custody of the tokens, the system accepts deposits of approved native tokens to isolate/remove said native tokens from circulation to keep them *safeguarded from theft and protected from quantum threats within the ur369.eth smart contract*, while simultaneously, upon receiving native tokens, the system mints urTokens (ultra resistant Tokens) and automatically sends urTokens to the user's wallet at 1:1 ratio in regards of the protected native tokens. 

On the edge of the coin, it is a self-organizing distributive-system as in the process of protecting the native tokens plus issuing-and-sending urTokens (ultra resistant Tokens) to the user's wallet >> the system shows (upfront) to the user a benefaction-fee for the service provided (i.e., a fix 0.369% of the amount to be deposited/protected) from which, if the user consents and pays the service-fee to protect their native tokens, then the system programmatically distributes the 0.369% benefaction-fee into 4 addresses as follows (A) 30% to fund public goods (so far on payroll Giveth, Gitcoin and the Giving Block), (B) 30% to award randomly selected end-users every 369 hours, (C) 30% to self-sustain the social good protocol (ur369.eth) and (D) 10% to support the Community and Developers Benefit Fund.

**_Procedure_**

- Once on the UI dashboard, the user clicks on the 'Protect' button corresponding to the native token they want to protect.
  
- The system will check if this is a new user/address or not. In case of an already registered user/address the system just shows the form for the user to allocate the desired amount of native tokens into the contract to be protected.

- In case of new user/address the system will randomly generate an encrypted Master Key for the user (only shown once on that section and during that time) and will prompt the user to set a Sign Key or a Quantum Resistant Sign Key (optional). 

- The Master Key will be used to (A) recover the user's Sign Key in case it is lost or forgotten and (B) for the user to add Quantum Key (in case the user did not add it in the first instance and wanted to add it later).

- Therefore, previous to jumping into setting the Sign Key, the system clearly indicates to the user a step-by-step guide to safely export the provided and encrypted Master Key from online to offline with: (A) near zero chances of misspelling it (as the Master Key is comprised of seperators, placed every 5 characters, to facilitate its clear reading and transcription) and (B) lowering the posibility for the Master Key to be remotely viewed or detected by a possible/potential bad actor as the system, before displaying the Master Key on the screen: (i) advises the user to have the internet off, and (ii) the system also alerts to never take a picture or screenshot of the Master Key or private keys.
    
- **_Instructions to safely export the Master Key from online to offline (the 8 steps below are out of the scope of the code - however, these are included here as they can help anyone to fully understand the hollistic approach to best parctice in Crypto Security and the overall rationale):_**
  
- *_(1) Turn off the Wi-Fi / Internet connection_*
- *_(2) Check the box to acknowledge the WiFi/internet is off - as only after the user acknowledges the internet is off is when the user can click a button/icon to make the Master Key visible_*
- *_(3) The system indicates the user to write the Master Key on a piece of paper (temporarily); and instructs that the optimal way to store the Master Key (as well as private Keys) is a solid, stainless, acid-resistant, shockproof, and fireproof piece of metal_*
- *_(4) Double/triple check for any misspelling(s)_*
- *_(5) Click button/icon to show the Master Key encrypted again_*
- *_(6) Turn on the Wi-Fi_*
- *_(7) Check the box(es) 'Add Quantum Resistant Protection (Optional)' and 'I understand ur369.eth cannot recover the Sign Key for me'_*
- *_(8) The user sets Sign Key (a strong password or PIN that the user selects on their end to abstract away the private keys and protect tokens from theft) or the user sets a Quantum Resistant Sign Key (a strong password or PIN that the user selects on their end -- for this option the system incorporates a Dilithium Crystrals Algorithim) to abstract away the private keys and protect tokens from quantum threats*
  
- ## Code functionality resumes and continues on the next step
  
- In regards to point 8 above >> only after the user has acknowledged and checked the respective boxes 'Add Quantum Resistant Protection (optional)' and 'I understand ur369.eth cannot recover the Sign Key for me' is that the user can continue to 'Set Sign Key' and click on 'Enable Sign Key'.

- After clicking 'Enable Sign Key' the user signs the transaction on their wallet. When the transaction is confirmed onchain the system pairs and saves the Master Key and the Sign Key.

- The UI presents a pop-up for the user showing they have enabled Classical Sign Key or the Quantum Resistant Sign Key and provides the user with a hyperlink for them to see the transaction on the block explorer.

- On the block explorer the user can see the onchain call function 'Set Master Key And Sign Key' if classical Sign Key was enabled; or the user can see 'Set Master Key And Quantum Resistant Sign Key' if the Quantum Resistant Key was the option selected.

- When the user comes back to the UI and closes the pop-up with previous transaction (re enabling Sign Key), the UI presents a modal to enter the desired amount of native tokens the user wants to protect.

- The user inputs the amount of native tokens they want to protect (allocate into the contract), the UI shows the benefaction-fee of 0.369% that the user must pay in order to execute the operation. The UI shows the amount of urTokens (ultra resistant Tokens) the user will receive; for example, if the user is allocating ETH the user will receive urETH at 1:1 ratio after the benefaction-fee.

- If all is ok on the user's end, then the user inputs their Sign Key and confirms the transaction on their wallet.

- After the transaction is confirmed, the UI shows the amount of native tokens protected (allocated within the contract), the benefaction-fee amount the user paid to the contract, the amount of urTokens the contract issued and sent to the user's account. The UI also provides the user with a hyperlink for them to see and inspect the transaction details on the block explorer.

- On the block explorer the user can see all details as stated above and also how the benefaction fee they paid was automatically distributed into 4 addresses ((1)urgift / (2)ur-impact / (3)ur369 / (4)ur-community & devs benefit fund).

- Once protected, the user can unportect and withdraw the native tokens at anytime and without restrictions. For this the user only has to click on 'Claim' button and proceed to burn the desired amount of urTokens and they automatically receive the native tokens into their wallet.
  

### Transferring urTokens

**_Definition:_** urTokens can be transfered if-and-only-if the user enters their respective Sign Key. Protected tokens can be permissionlessly transfered by the legit owners at any time and without restrictions.

**_Procedure_**

- Click on "Transfer" button corresponding to tne respective urToken field
- Enter the amount of urTokens to transfer
- Enter recipient address
- Input respective Sign Key
- Click 'Transfer' button and confirm the Tx on the wallet


### Unprotecting (claiming) Native Tokens

**_Description:_** Unprotecting native tokens from the ur369 smart contract to receive native tokens back into your wallet. This operation is executed by burning urTokens and automatically receiving native tokens at 1:1 ratio back into your wallet.

**_Procedure_**

- Click on "Claim" button corresponding to tne respective urToken field
- Enter desired amount to unprotect
- Enter the respective Sign Key and click on 'Unprotect' button
- Smart contract will burn entered amount of urTokens and the respective native tokens will be transferred back into the user's wallet at 1:1 ratio
- The user can unprotect (claim) native tokens at any time and without restrictions
  

### Benefaction-Fee Collection System

**_Description:_** Each time a user protects/allocates native tokens within the contract, a specific and fix percentage (0.369%) will be deducted from the entered amount >> converted into urToken and sistributed across the system to fulfill a purpose. The remaining amount of native tokens will be safeguarded within the contract and the respective 1:1 ratio is minted and sent into the user's account.


**_Fee Collectors_**

1. 30% of 0.369% will be transferred to the urgift.eth address which will send awards to randomly selected participants every 369 hours 
2. 30% of 0.369% will be transferred to the ur-impact.eth to fund public goods and other important causes for the ecosystem
3. 30% of 0.369% will be transferred to the ur369.eth address to self-sustain the social good
4. 10% of 0.369% will be transferred to the ur369community-devs.eth address to support the ur369.eth Community & Developers Benefit Fund

   **_Procedure_**

- Fee will be deducted at time time of protecting native tokens.
  

### Awward System

**_Description:_** Upon start of each time period, a random participant address will be selected which will receive an award from the collected % of previous received benefaction-fees and from awards non-collected by users in previous rounds / time periods. 

*_If the system is being used and there are funds within the respective addresses to distribute awards >> the awards shall arrive to the randomly selected ones._*

**_Procedure_**

- Smart contract collects benefaction-fee and send 30% of benefaction fee to urgift.eth (award address) and send 30% to ur-impact.eth
- Each detail will be shown on the 'Award' page regarding collectable assets
- The randomly selected participant's address will be shown in the Awards page
- Smart contract will transfer all the collected benefaction-fee to the respective addresses urgift.eth (award address) and send 30% to ur-impact.eth and here stops/end the code functionality

- Note: The rest of the procedure with respect of 'Awards' is outside of the code's scope and is bound to a game theoretical approach that can be seen in the 'Award' page ('Gift Pool' and "Stateless Pool' stated conditions) >> those transactions to send awards are performed manually (the reason for this approach can be found in the ur369.eth.limo UI (Insight page -- point (14)). The transparent nature of the blockchain(s) where urTokens are deployed will attest for the fullfilment of these manual transactions.


### Whitelist Mechanism

**Definition:** Whitelist users can enter the Sign Key to perform a transaction (send urToken) from UI. Whitelisted smart contract(s) does not have to input Sign Key to transfer urTokens. 

**Implementation Guide:**
Implementation can be usderstand in two ways.

Sender is Uniswap or AAVE (Uniswap is whitelisted):
   The system checks if the sender is a whitelisted contract address, and then the system allows for it to transfer urTokens without having to input Sign Key.

**Strategy to Implement Whitelist Functinality:**
There are two ways to check that caller is a contract address or not:

- if(msg.sender == tx.origin): in case of true, caller is EOA otherwise caller is a contract.
- if(msg.sender.code.length == 0): in case of true, caller is an EOA otherwise caller is a contract.
- **_Note:_**
  1. Any of above can be used to check whether caller is an EOA or a contract.
  2. isContract() function of Address Library is deprecated due to security reasons.


### Sign Key to perform transactions

**_Description:_** To prevent users from transferring urTokens directly from any wallet, the feature has been implemented. On each user operation involving urTokens 'Transfer' or 'Claim' >> the user must enter their respective Sign Key on the UI otherwise transaction will fail.


### Master Key as Recovery Mechanism

**_Description:_** If the user forgot or lost the Sign Key, the user can come to the UI, input their Master Key and reset the Sign Key. 

**_Procedure_**

- Click on "Forgot Sign key"
- Turn off any Wi-Fi / internet connection
- *With the internet off* input the Master Key into the respective field: include all the separators ( - ) *up to the last dash/separator* and leave no spaces in between the dashes and the letters/characters, it shall all look as a string of dots -encrypted-
- *Important: make sure you leave out (do not type) the last 4 characters.*
- Turn the internet ON and with the cursor at the very end of the Master Key >> input the last 4 characters of the Master Key and click enter
- The field "Reset Sign Key" to input and confirm new Sign Key should display for you

### Important note

In the beginning and even before allocating funds into the contract, you can use the same procedure as above to confirm that your Sign Key has been transcribed correctly. Becaue when you apply those steps and you see the outcome 'The field "Reset Sign Key" to input and confirm new Sign Key should display for you', that means that you have transcribed your Master Key Correctly and you can allocate funds with 100% confidence into the contract. Keep the Master Key a;ways in a safe place (preferably offline).


### Quantum Resistant Approach

**_Overview_**

With the advancements in quantum computing, traditional cryptographic approaches are becoming increasingly vulnerable. To future-proof the ecosystem, the Dilithium-Crystals quantum-resistant algorithm is used.

**_Implementation Flow_**

### Hashing with Keccak-256

First the Master Key and the Sign Key are hashed with Keccak-256, a reliable algorithm widely used in blockchain, to add another layer of security.

### Applying Quantum-Resistant Signature (Dilithium-Crystals)

Upon enabling the Master Key and Sign Key, a Dilithium-Crystals signature is generated, ensuring a high level of quantum security. This signature, together with the public key, is stored on the blockchain, creating a secure reference point for future verification.

### Signing with the crypto wallet Private Key

The Keccak-256 hash is signed using the user’s wallet private keys, which authenticates the transaction on the blockchain and adds an extra verification layer.

### Storing Data on Blockchain

The Dilithium-Crystals signature, public key, Keccak-256 hash, and the wallet signature are securely stored on the blockchain. To ensure authenticity, the Wallet signature is verified using the ecrecover function, validating the signature against the user’s address.

### Sign Verification Process

To sign, the user enters their Sign key, and the Keccak-256 hash is regenerated. This hash is then compared against the stored data on the blockchain. A new Wallet signature is created and verified on-chain.

### Rationale for selecting Dilithium-Crystals among other NIST-recommended algorithms

NIST recommends multiple quantum-resistant algorithms, including SPHINCS+, Rainbow, Dilithium-Crystals etc. Here’s why it has been selected: Dilithium-Crystals offers efficient storage, consistent key generation, and resilient security against both classical and quantum attacks.

### Multi-Layered Security

To maximize security, ur369.eth implements three distinct layers of protection:

### Front-End Quantum-Resistant Signature: 

Dilithium-Crystals applied on the front end ensures protection against quantum threats.

### Backend Keccak Hash: 

The Keccak-256 hash provides backend-level protection, safeguarding the Master Key and the Sign Key on-chain.

### Frontend-Backend Connection Verification: 

Works for both Classic and Quantum Protection, thus by requiring the Sign Key and/or the Quantum Resistant Sign Key (when enabled) to sign >> unauthorized direct access is prevented, ensuring that only onchain-verified-users can interact with the application.

Note: Onchain-verified users does not relate nor indicates KYC (Know Your Customer); the onchain-verification, in this context, means the users having created their Sign Key and/or their Quantum Resistant Sign Key (optional).

