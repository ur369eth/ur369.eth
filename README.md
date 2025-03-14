**ur369 (ultra resistant 369)** 
**urTokens (ultra resistant Tokens)** 
**Functionality is described in Code**

Description of working of Smart Contract is as follows:

## Functionalities

- Decentralized Protection of Native Tokens
- Fee Collection System (Benefaction-fee)
- Award System (Hybrid)
- Sign Key to Perform User Operations (Transactions)
- Transfer urTokens (ultra resistant Tokens)
- Decentralized Unprotection of Native Tokens (Claim)
- Whitelist Mechanism for Smart Contracts (Interop)
- Master Key as Recovery Mechanism
- Quantum Resistant Approach

### Decentralized Protection of Native Tokens


**_Definition:_** For a comprehensive definition, let's use the following verbal illustration:

**On one side of the coin >>** this is independent onchain 2FA (with extra functionalities). The main objective is to help prevent (and stop in full) crypto theft caused by bad actors infesting the ecosystem with constant phishing attacks, wallet drainers, and with other sophisticated exploits (see Bybit hack). The scope of the protection includes *potential quantum threats* (incorporating Dilithium-Crystals into the security scheme).

It works by allowing the user to set (and confirm onchain) their own Classical Sign Key (or a Quantum Resistant Sign Key) to abstract away the wallet's private keys to sign transactions.

**On the other side of the coin >>** this is a mechanism in wich, without having a centralized custody of any token, the system accepts deposits of approved native tokens to isolate/remove said native tokens from circulation to keep them *safeguarded from theft and protected from quantum threats within the ur369.eth smart contract*, while simultaneously, upon receiving native tokens, the system mints urTokens (ultra resistant Tokens) and automatically sends urTokens to the user's wallet at 1:1 ratio in regards of the protected native tokens. 

**On the edge of the coin >>** this is a self-organizing distributive-system, because before the process of protecting the native tokens plus issuing-and-sending urTokens to the user's wallet, the system shows (upfront) to the user the benefaction-fee for the service provided:

(i) A one time flat fee of $3.69 per address -collected in crypto- and only charged if the user opts for the Quantum Resistant Key.

(ii) And a 0.369% of the amount being protected -collected each time the user allocates funds within the contract-.

If the user consents and pays the benefaction-fee to protect their native tokens, then when the system receives it >> programmatically distributes the benefaction-fee into 4 addresses as follows: 

(A) 30% to fund public goods (so far on payroll Giveth, Gitcoin and the Giving Block -more public goods can be added later-)  
(B) 30% to award randomly selected users every 369 hours  
(C) 30% to self-sustain ur369.eth (the social good protocol) and  
(D) 10% to support the Community and Developers Benefit Fund  

**_Procedure_**

- Once on the UI dashboard, the user clicks on the 'Protect' button corresponding to the native token they want to protect.
  
- The system will check if this is a new user/address or not. In case of an already registered user/address the system just shows the form for the user to allocate the desired amount of native tokens into the contract to be protected.

- In case of new user/address the system will randomly generate an encrypted Master Key for the user (only shown once on that section and during that time) and will prompt the user to set a Sign Key or a Quantum Resistant Sign Key (optional). 

- The Master Key will be used to (A) recover the user's Sign Key in case it is lost or forgotten and (B) for the user to add Quantum Key (in case the user did not add it in the first instance and wanted to add it later).

- Therefore, previous to jumping into setting the Sign Key, the system clearly indicates to the user a step-by-step guide to safely export the provided and encrypted Master Key from online to offline with: (A) near zero chances of misspelling it (as the Master Key is comprised of seperators, placed every 5 characters, to facilitate its clear reading and transcription) and (B) lowering the posibility for the Master Key to be remotely viewed or detected by a possible/potential bad actor as the system, before displaying the Master Key on the screen:

- (i) Strongly recommends the user to have the internet off
- (ii) On purpuse, the system does not provide a "copy Master Key button" in the UI, thus inducing the user to export the Master Key by writing it offline instead of copying it as that practice could carry a risk vector, and
- (iii) The system also alerts to never take a picture or screenshot of the Master Key or private keys
    
- **_Instructions to safely export the Master Key from online to offline (the 8 steps below are out of the scope of the code - however, these are included here in order to assist with the full understanding of the hollistic approach about best parctice in Crypto Security and the overall rationale):_**
  
- *_(1) Turn off the Wi-Fi / Internet connection_*
- *_(2) Check the box to acknowledge the WiFi/internet is off - as only after the user acknowledges the internet is off is when the user can click a button/icon to make the Master Key visible_*
- *_(3) The system indicates the user to write the Master Key on a piece of paper (temporarily); and instructs that the optimal way to store the Master Key (as well as private Keys) is a solid, stainless, acid-resistant, shockproof, and fireproof piece of metal_*
- *_(4) Double/triple check for any misspelling(s)_*
- *_(5) Click button/icon to show the Master Key encrypted again_*
- *_(6) Turn on the Wi-Fi_*
- *_(7) Check the box(es) 'Add Quantum Resistant Protection (Optional)' and 'I understand ur369.eth cannot recover the Sign Key for me'_*
- *_(8) The user sets Sign Key (a strong password or PIN that the user selects on their end to abstract away the private keys and protect tokens from theft) or the user sets a Quantum Resistant Sign Key (a strong password or PIN that the user selects on their end -- for this option the system incorporates a Dilithium Crystrals Algorithim) to abstract away the private keys and protect tokens from quantum threats*
  
- ## Code functionality resumes and continues on the next fields
  
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


### Benefaction-Fee Collection System

**_Description:_** Two types of benefaction-fee are charged for the protect-service provided. The protcol always shows the fee upfront before collecting them:

(i) A flat amount equivalent to $3.69 (collected in crypto and only once per address); this flat fee-amount is only charged if the user opts for the Quantum Resistant Sign Key. Upon collection the system automatically distributes the flat amount fee to 4 designated address with a social-good-purpose.

(ii) A specific 0.369% of the amount the user wants to protect/allocate within the contract. This fee is collected by the system every time the user is protecting native tokens.

As the system always shows the fee amount upfront to the user in the UI and as the user becomes aware of the benefaction-fee, then when the user proceeds to protect native tokens >> the benefaction-fee is deducted from the entered amount and the fee is distributed across 4 addresses within the system to fulfill a social-good-purpose. The remaining amount of native tokens is safeguarded within the contract and the equal amount of urTokens are minted-and-sent to the user's wallet address at 1:1 ratio in regards of the safeguarded native tokens. 

Clarifying example: If after fee the user has 369 ETH within the contract then for this user the system minted-and-sent 369 urETH to the user's account.

In essence, the system charges the benefaction-fee when protecting tokens; but not for any other operations like 'Transfer' or 'Claim' (only the gas fee shall be paid to validators for those operations). 

**_Fee Collectors_**

1. 30% of 0.369% is transferred to the urgift.eth address which will send awards to randomly selected participants every 369 hours 
2. 30% of 0.369% is transferred to the ur-impact.eth to fund public goods and other important causes for the ecosystem
3. 30% of 0.369% is transferred to the ur369.eth address to self-sustain the social good protocol
4. 10% of 0.369% is transferred to the ur369community-devs.eth address to support the ur369.eth Community & Developers Benefit Fund

   **_Procedure_**

- First the fee is shown to the user before protecting their native tokens. When the user proceeds to protect their native tokens >> the benefaction-fee is deducted and distributed to the respective addresses for social-good-purpose.
  

### Awward System

**_Description:_** Every time a user protects native tokens the system charges a Benefaction-fee which is used, in its great majority, to award to the participants of the system and the rest is used for public goods funding.

Every 369 hours (Gift Pool) and every 369 days (Stateless Pool) a participant that protected native tokens will be randomly selected and their address will be displayed on the UI in a semi-concealed fashion. 

**_Procedure_**

- Smart contract collects benefaction-fee and sends 30% to urgift.eth and 30% to ur-impact.eth
- Each detail will be shown on the 'Award' page regarding the assets that can be awarded to users and that are within the displayed addresses
- The randomly selected participant's address will be shown in the Awards page every 369 hours in a semi-concealed fashion
  
*_Note: The award system is hybrid, meaning that the above is within the scope of the code. However, for the part shared below, in regards of this segment of 'Award System' the code functionality is not included as the next section for the Award System operation is executed manually. The reason for the manual approach can be found in the ur369.eth.limo UI -Insight page -- point (14)-._*

*_Just as a courtesy and honoring transparency, here is shared the Award System Manual approach:_*

*_The objective is to avoid a sybil exploit that can be effected if the system send awards automatically via code (as it was found while testing) and the purpose is for the participants to receive awards without any possibility of them tricking the system. Awards can be sent from: (A) the Gift Pool, (B) the Impact Pool, (C) the Stateless Pool (any award for A, B and C is received by the user if they fulfilled the stated pool conditions - see Awards page), and (D) to receive awards from satellite-addresses that work in harmony with the ur369NFT mint._* 

*_The transparent nature of a public blockchain (like Ethereum) where urTokens are deployed, can attest for the fullfilment of these manual transactions that can be correlated and publicly audited to confirm that an address displayed in the UI, for example, did (or did not) mint the ur369NFT and did or did not receive the corresponding urTokens award if selected by the system._*

*_In conclusion, if the system is being used and there are funds within the respective addresses to distribute awards >> the awards shall arrive to the randomly selected ones._*

The code functionality continues in subsequent fields.


### Sign Key to Perform User Operations (Transactions)

**_Description:_** urTokens can be transferred if-and-only-if the user inputs the respective Sign Key.

The feature has been impelmented to serve as an extra layer of protection, primarily to prevent any bad actor from executing a transaction even if they would have gained access to the wallet's private keys of the user. Therefore, on each user operation involving urTokens 'Transfer' or 'Claim' >> the user must enter their respective Sign Key on the UI otherwise transaction will fail. Without the Sign Key urTokens cannot be moved.


### Transfer urTokens

**_Definition:_** urTokens can be transfered if-and-only-if the user enters their respective Sign Key. urTokens can be permissionlessly transfered by the legit owners at any time and without restrictions. 

The ur369.eth protocol does not charge a fee for this operation, only the gas fee must be paid by the users to validators of the respective chain.

**_Procedure_**

- Click on "Transfer" button corresponding to tne respective urToken
- Enter the amount of urTokens to transfer
- Enter recipient address
- Input respective Sign Key
- Click 'Transfer' button and confirm the transaction on the wallet
- When the transaction is confirmed onchain the UI shows the amount of urTokens being transferred
- The UI provides a hyperlink for the user to review the transaction details on the block explorer


### Decentralized Unprotection of Native Tokens (Claim)

**_Description:_** urTokens can be transfered if-and-only-if the user enters their respective Sign Key.

Unprotecting native is claiming the tokens from the ur369 smart contract to receive the native tokens back into the user's wallet. This operation is executed by burning urTokens and automatically receiving native tokens at 1:1 ratio back into the user's wallet. 

The ur369.eth protocol does not charge a fee for this operation, only the gas fee must be paid by the user to validators of the respective chain.

**_Procedure_**

- Click on "Claim" button corresponding to tne respective urToken
- Enter desired amount to unprotect
- Smart contract will show the amount of urTokens that will be burned and the amount of native tokens to be received into the user's wallet
- Enter the respective Sign Key, click 'Unprotect' button and confirm transaction on the wallet
- Smart contract burns entered amount of urTokens and the respective native tokens will be transferred back into the user's wallet at 1:1 ratio
- When the transaction is confirmed onchain, the UI shows the amount of urTokens burned and the amount of native tokens received
- UI provides the user with a hyperlink for the user to review the transaction details on the block explorer 
- The user can unprotect (claim) native tokens at any time and without restrictions


### Whitelist Mechanism for Smart Contracts (Interop)

**Definition:** The user can enter the Sign Key on the UI to perform any transaction with urTokens. However, whitelisted smart contract(s) will not have to input the respective Sign Key to internally or externally transfer urTokens. 

**Implementation Guide:**

For example, the sender is Uniswap or AAVE (Uniswap v4 (Hooks) is actually whitelisted on the Ethereum mainnet):
   The system checks if the sender is a whitelisted contract address, and then the system allows for it to transfer urTokens without having to input Sign Key.

**Strategy to Implement Whitelist Functionality:**
There are two ways to check that caller is a contract address or not:

- if(msg.sender == tx.origin): in case of true, caller is EOA otherwise caller is a contract.
- if(msg.sender.code.length == 0): in case of true, caller is an EOA otherwise caller is a contract.
- **_Note:_**
  1. Any of above can be used to check whether caller is an EOA or a contract.
  2. isContract() function of Address Library is deprecated due to security reasons.


### Master Key as Recovery Mechanism

**_Description:_** If the user forgot or lost the Sign Key, the user can come to the UI, input their Master Key and reset the Sign Key. 

**_Procedure_**

- Click on "Forgot Sign key"
- Turn off any Wi-Fi / internet connection
- *With the internet off* input the Master Key into the respective field: include all the separators ( - ) *up to the last dash/separator* and leave no spaces in between the dashes and the letters/characters, it shall all look as a string of dots -encrypted-
- *Important: make sure you leave out (do not type) the last 4 characters.*
- Turn the internet ON and with the cursor at the very end of the Master Key >> input the last 4 characters of the Master Key and click enter
- The field "Reset Sign Key" to input and confirm new Sign Key should display for the user

### Important note

In the beginning and even before allocating funds into the contract, the user can use the same procedure as described above to confirm that their Sign Key has been exported from online to offline correctly. 

When these steps are applied and the user can see the field 'Reset Sign Key' to input and confirm new Sign Key, that means the Master Key has been transcribed without any misspellings and the user can allocate funds with 100% confidence into the contract.

The Master Key must always be kept in a safe place (preferably offline).


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

The user enters their Sign key, and the Keccak-256 hash is regenerated. This hash is then compared against the stored data on the blockchain. A new Wallet signature is created and verified on-chain.

### Rationale for selecting Dilithium-Crystals among other NIST-recommended algorithms

NIST recommends multiple quantum-resistant algorithms, including SPHINCS+, Rainbow, Dilithium-Crystals, etc. Here’s why it has been selected: Dilithium-Crystals offers efficient storage, consistent key generation, and resilient security against both classical and quantum attacks.

### Multi-Layered Security

To maximize security, ur369.eth implements three distinct layers of protection:

### (1) Front-End Quantum-Resistant Signature: 

Dilithium-Crystals applied on the front end ensures protection against quantum threats.

### (2) Backend Keccak Hash: 

The Keccak-256 hash provides backend-level protection, safeguarding the Master Key and the Sign Key on-chain.

### (3) Frontend-Backend Connection Verification: 

This works for both Classical and Quantum Protection, thus by requiring the Classical Sign Key or the Quantum Resistant Sign Key (when enabled) to sign then any unauthorized direct access is prevented, ensuring that only onchain-verified-users can interact with the application.

