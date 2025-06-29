# What is ur369.eth.limo?

ur stands for **ultra resistant** -- ur369.eth.limo is the distributed access point -User Interface (UI)- of the non-custodial and decentralized smart contract built for the purpose of: 
- protect cryptographic tokens from theft and quantum threats
- award users every 369 hours
- fund public goods


# What are urTokens (ultra resistant Tokens)?

urTokens are ERC-20 tokens backed by cryptographic tokens at 1:1 ratio. Exegesis: if a user allocates 369 ETH into the contract, then the contract automatically mints and sends 369 urETH (ultra resistant ETH) to their wallet address.

Advantage of urTokens over native tokens and/or ERC-20 tokens as well as over any other token-standard (e.g., BEP-20, SPL, etc):

(A) urTokens can only be transferred if-and-only-if the user inputs their Sign Key which they previously set (and confirmed onchain), making urTokens ultra resistant to theft.

(B) urTokens protect themselves and protect the cryptographic tokens within the contract from quantum threats with Dilithium-Crystals (a highly secure and efficient Post Quantum Cryptography (PQC) algorithm with a small signature scheme - suitable to use in blockchain).

(C) The users holding urTokens are always elegible to receive random awards from the system.


# Smart Contract -- Functionality is Described in Code

Description of working of Smart Contract is as follows:

### Functionalities

- Decentralized Protection of Cryptographic Tokens (369)
- Fee Collection System (Benefaction-fee)
- Award System (Hybrid)
- Sign Key to Perform User Operations (Transactions)
- Transfer urTokens (ultra resistant Tokens)
- Decentralized Unprotection of Cryptographic Tokens (Claim)
- Whitelist Mechanism for Smart Contracts (Interop)
- Master Key as Recovery Mechanism (Lost/forgotten Sign Key)
- Quantum Resistant Approach (Dilithium-Crystals)

### Decentralized Protection of Cryptographic Tokens

**_Definition:_** Let's share a comprehensive definition from three factual perspectives (3/6/9) using "a coin" for verbal illustration:

**(3) On one side of the coin >>** this is an independent onchain 2FA (with extra functionalities). The main objective is to help prevent (and stop in full) the theft of cryptogrpahic tokens (also called crypto tokens or tokens); such theft is widely caused by bad actors infesting the crypto ecosystem with constant phishing attacks, wallet drainers, and with other sophisticated exploits (see Bybit hack). 

The scope of the *decentralized protection* of crypto tokens includes *potential quantum threats* (incorporating Dilithium-Crystals into the security scheme).

The decentralized protection of crypto tokens works by allowing the users to set (and confirm onchain) their own Classical Sign Key (and also Quantum Resistant Sign Key -optional-) to abstract away the wallet's private keys to sign transactions.

**(6) On the other side of the coin >>** this is a mechanism in wich, without having any centralized custody of any crypto token, the system accepts deposits of approved crypto tokens to isolate/remove said crypto tokens from circulation to keep them *safeguarded from theft and protected from quantum threats within the smart contract*, and simultaneously, upon receiving crypto tokens, the system mints urTokens (ultra resistant Tokens) and automatically sends urTokens to the user's wallet address at 1:1 ratio in regards of the protected crypto tokens. 

**(9) On the edge of the coin >>** this is a self-organizing and self-sustaining distributive-system, because before-and-for this process to be accomplished (i.e., the decentralized protection of crypto tokens plus issuing-and-sending urTokens to the user's wallet) >> the system shows (upfront) to the user >> the benefaction-fee for the protection-service provided:

(i) A $3.69 benefaction-fee, collected in the native token of the chain, **_charged only once per wallet addres and only if the user opts for the Quantum Resistant Sign Key._**

(ii) A $3.69 benefaction-fee collected in the native token of the chain **_charged every time the user alloctates a crypto asset within the contract to protect against theft_**.

When the system receives the benefaction-fee >> programmatically distributes the funds into 4 addresses as follows: 

(A) 30% to the Impact Pool (ur-impact.eth) to fund public goods (e.g., Giveth, Gitcoin, the Giving Block, Open Sats...) and to award ideas providers (IPs).

(B) 30% to the Gift Pool (urgift.eth) to award randomly selected users every 369 hours

(C) 30% to ur369self-sustain.eth for the sustenance of ur369.eth (the social good protocol) 

(D) 10% to ur369community-devs.eth to support the Community and Developers Benefit Fund 

Note: For this last part the code works up to sending funds to the corresponding addresses for A, B, C and D -- the subsequent transfers from said addresses are outside of the scope of this code and the transparent nature of the chain shall attest of said transfers (after the transfers are effected and confirmed onchain). The reason for this manual-transactions after funds are received into the respective addresses programatically, can be found in the ur369.eth.limo UI -Insight page, point (14).

**_Procedure_**

- Once on the UI dashboard, the user clicks on the 'Protect' button corresponding to the crypto token they want to protect
  
- The system will check if this is a new user/address or not. In case of an already registered user/address the system just shows the form for the user to allocate the desired amount of tokens into the contract to be protected

- In case of new user/address the system will randomly generate an encrypted Master Key for the user (only shown once on that section and during that time) and will prompt the user to set a Sign Key or a Quantum Resistant Sign Key (optional)

- The Master Key will be used to (A) recover the user's Sign Key in case it is lost or forgotten and (B) for the user to add Quantum Resistant Sign Key (in case the user did not add it in the first instance and wanted to add the Quantum Key later)

- Therefore, previous to proceeding to setting the Sign Key, the system clearly indicates to the user a step-by-step guide to safely export the provided and encrypted Master Key from online to offline with: (A) near zero chances of misspelling it (as the Master Key is comprised of seperators, placed every 5 characters, to facilitate its clear reading and transcription) and (B) with near zero chances for the Master Key to be remotely viewed or detected/intercepted by any potential bad actor; as the system, before allowing the Master Key to be visible on the screen:

- (i) Indicates and strongly recommends the user to turn the internet off, and the Master Key **can only be viewed after the user checks a box to acknowledge the internet is off**
- (ii) On purpuse, the system does not provide a "copy Master Key button" in the UI, thus inducing the user to export the Master Key by writing it offline instead of copying the Master Key as the practice of copying the Master Key could carry a risk vector, and
- (iii) The system also alerts to never take a picture or screenshot of the Master Key
    
- **_Instructions to safely export the Master Key from online to offline (the 8 steps below are out of the scope of the code - however, these are included here in order to assist with the full understanding of the hollistic approach about best parctice in Crypto Security and the overall rationale):_**
  
- *_(1) Turn off the Wi-Fi / Internet connection_*
- *_(2) Check the box to acknowledge the WiFi/internet is off - as only after the user acknowledges the internet is off is when the user can click a button/icon to make the Master Key visible_*
- *_(3) The system indicates the user to write the Master Key on a piece of paper (temporarily); and instructs that the optimal way to store the Master Key (as well as private Keys) is a solid, stainless, acid-resistant, shockproof, and fireproof piece of metal_*
- *_(4) Double/triple check for any misspelling(s)_*
- *_(5) Click button/icon to show the Master Key encrypted again_*
- *_(6) Turn on the Wi-Fi_*
- *_(7) Check the box(es) 'Add Quantum Resistant Protection (Optional)' and 'I understand ur369.eth cannot recover the Sign Key for me'_*
- *_(8) The user sets Sign Key (a strong password or PIN that the user selects on their end to abstract away the private keys and protect tokens from theft) or the user sets a Quantum Resistant Sign Key (a strong password or PIN that the user selects on their end -- for this option the system incorporates a Dilithium Crystrals Algorithim) to abstract away the private keys and protect tokens from quantum threats_*
  
- ## Code functionality resumes and continues on the following fields
  
- In regards to point 8 above >> only after the user has acknowledged and checked the respective boxes 'Add Quantum Resistant Protection (optional)' and 'I understand ur369.eth cannot recover the Sign Key for me' is that the user can continue to 'Set Sign Key' and click on 'Enable Sign Key'.

- After clicking 'Enable Sign Key' the user signs the transaction on their wallet. When the transaction is confirmed onchain the system pairs and saves the Master Key and the Sign Key.

- The UI presents a pop-up for the user showing they have enabled Classical Sign Key or the Quantum Resistant Sign Key (if this was the selected Key to sign) and provides the user with a hyperlink for them to review the transaction on the block explorer.

- On the block explorer the user can see the onchain-call-function 'Set Master Key And Sign Key' if classical Sign Key was enabled; or the user can see 'Set Master Key And Quantum Resistant Sign Key' if the Quantum Resistant Key was the option selected.

- When the user comes back to the UI and closes the pop-up with previous transaction (re enabling Sign Key), the UI presents a modal to enter the desired amount of tokens the user wants to protect.

- The user inputs the amount of tokens they want to protect (allocate into the contract), the UI shows the benefaction-fee of $3.69 that the user must pay in crypto in order to execute the 'Protect' operation. The UI shows the amount of tokens the user will allocate within the contract and the amount of urTokens (ultra resistant Tokens) the user will receive in their connected wallet address at 1:1 ratio.

- To send the transaction >> the user must input their Sign Key and confirm the transaction on their wallet.

- After the transaction is confirmed, the UI shows the amount of crypto tokens protected (allocated within the contract), the benefaction-fee amount the user paid to the contract, the amount of urTokens the contract issued and sent to the user's account. The UI also provides the user with a hyperlink for them to see and inspect the transaction details on the block explorer.

- On the block explorer the user can see all details as stated above and also how the benefaction fee they paid was automatically distributed into the 4 addresses: (1)urgift.eth / (2)ur-impact.eth / (3)ur369self-sustain.eth / (4)ur369community-devs.eth).

- Once protected, the user can unportect and withdraw the crypto tokens at anytime and without restrictions. For this operation the user only has to click on 'Claim' button and proceed to burn the desired amount of urTokens and they automatically receive the corresponding crypto tokens into their wallet.


### Benefaction-Fee Collection System

**_Description:_** Two types of benefaction-fee are charged for the provided service of protecting the crypto assets. The protcol always displays and inform about the fee upfront, thus the user becomes aware of the fee to be paid:

(i) The Quantum Resistant Protection: A $3.69 fee collected in the native token of the chain **_only once per wallet address._** Enabling the Quantun Resistant Sign Key (to protect against quantum threats) is optional, and it can be activated at the beginning of the wallet address interaction with the protocol or at any future time as the user would desire.

(ii) The Classical Anti-Theft Protection: A $3.69 fee collected in the native token of the chain **_every time the user protects a crypto asset against theft_**. 

Upon collection of any of the fee type >> the system automatically distributes the flat amount fee to 4 designated address with a social-good-purpose.  

In essence, the system charges the benefaction-fee when protecting tokens; but does not charge a fee for any other User Operations like 'Transfer' or 'Claim' (only the gas fee shall be paid to validators for those operations). 

**_Fee Collectors_**

Every time the system collects in crypto the benefaction-fee equivatente to $3.69 -- then, programatically:

1. 30% is transferred to urgift.eth which will send awards to randomly selected users every 369 hours 
2. 30% is transferred to ur-impact.eth to fund public goods and other important causes for the ecosystem
3. 30% is transferred to ur369self-sustain.eth to self-sustain the social good protocol
4. 10% is transferred to ur369community-devs.eth to support the ur369.eth Community & Developers Benefit Fund

   **_Procedure_**

- First the fee is shown to the user before protecting their crypto tokens. The user can select the desired token to pay the fee, from stablecoins to a variety of tokens listed in the UI can be used to pay the fee.
- The user executes the transaction sending the benefaction-fee and the crypto asset to protect
- The fee is received into the system and automatically distributed to the respective addresses for social-good-purpose
- The user receives the urTokens (ultra resistant Tokens) at 1:1 ratio in regards of the crypto tokens they protected within the contract
- The urTokens sent to the user are visible and can be operated (e.g., transfer, claim) via the user interface (UI). To see the urTokens in their wallet, the user can click the 'Add to Wallet' button
  

### Awward System

**_Description:_** Every time a user protects crypto assets the system charges a Benefaction-fee, which is used, in its great majority, to award the participants of the system and the rest is used for public goods funding and to self-sustain the protocol.

Every 369 hours (Gift Pool) and every 369 days (Stateless Pool) a participant that protected any supported crypto asset(s) will be randomly selected and their address will be displayed on the UI in a semi-concealed fashion. If the user fulfilled the conditions to win the prize, then an award is sent to the user's wallet address.

**_Procedure_**

- Smart contract collects benefaction-fee and sends 30% to urgift.eth and 30% to ur-impact.eth
- Each detail will be shown on the 'Award' page regarding the assets that can be awarded to users and that are within the addresses urgift.eth and ur-impact.eth (displayed in the UI)
- The randomly selected participant's address will be shown in the Awards page every 369 hours, and for privacy-preserving reasons, the wallet address is displayed in a semi-concealed fashion
  
*_Note: The award system is hybrid, meaning that the above is within the scope of the code. However, for the part shared below, in regards of this segment of 'Award System' the code functionality is not included as the next section for the Award System Operation is executed manually. The reason for the manual approach can be found in the ur369.eth.limo UI -Insight page -- point (14)-._*

*_Just as a courtesy and honoring transparency, here is shared the Award System Operation (Manual Approach):_*

*_The objective is to avoid a sybil exploit that can be effected if the system sends awards automatically via code (the sybil exploit was found while testing) and the purpose is to eliminate the exploit and for the participants to receive awards without any possibility for them tricking the system. Awards can be sent from: (A) the Gift Pool, (B) the Impact Pool, and (C) the Stateless Pool (any award for A, B and C is received by the user if they completed their respective tasks and fulfilled the stated pool conditions - see Awards page 'Conditions to get the award' section). 

*_The transparent nature of a public blockchain (like Ethereum) where urTokens are deployed, can attest for the fullfilment of these manual transactions that can be correlated and publicly audited to confirm that an address displayed in the UI, for example, did (or did not) mint the ur369NFT and did or did not receive the corresponding urTokens award if selected by the system._*

*_In conclusion, if the system is being used and there are funds within the respective addresses to distribute awards >> the awards shall arrive to the randomly selected ones._*

The code functionality continues in subsequent fields.


### Sign Key to Perform User Operations (Transactions)

**_Description:_** urTokens can be transferred if-and-only-if the user inputs the respective Sign Key.

The feature has been impelmented to serve as an extra layer of protection, primarily to prevent any bad actor from executing a transaction even if they would have gained access to the wallet's private keys of the user. Therefore, on each user operation involving urTokens 'Transfer' or 'Claim' >> the user must enter their respective Sign Key on the UI otherwise the transaction will fail. Without the Sign Key urTokens cannot be moved.


### Transfer urTokens

**_Definition:_** urTokens can be transfered if-and-only-if the user enters their respective Sign Key. urTokens can be permissionlessly transfered by the legit owners at any time and without restrictions. 

The ur369.eth protocol does not charge a fee for the transfer operation, only the gas fee must be paid by the users to validators of the respective chain.

**_Procedure_**

- Click on "Transfer" button corresponding to tne respective urToken
- Enter the amount of urTokens to transfer
- Enter recipient address
- Input respective Sign Key
- Click 'Transfer' button and confirm the transaction on the wallet
- When the transaction is confirmed onchain the UI shows the amount of urTokens being transferred
- The UI provides a hyperlink for the user to review the transaction details on the block explorer


### Decentralized Unprotection of Cryptographic Tokens (Claim)

**_Description:_** urTokens can be transfered if-and-only-if the user enters their respective Sign Key.

Unprotecting crypto tokens is claiming (withdrawing) the tokens from the ur369 smart contract to receive the respective crypto tokens back into the user's wallet. This operation is executed by burning urTokens and automatically receiving crypto tokens at 1:1 ratio back into the user's wallet. 

The ur369.eth protocol does not charge a fee for this operation, only the gas fee must be paid by the user to validators of the respective chain.

**_Procedure_**

- Click on "Claim" button corresponding to tne respective urToken
- Enter desired amount to unprotect
- Smart contract will show the amount of urTokens that will be burned and the amount of crypto tokens to be received into the user's wallet
- Enter the respective Sign Key, click 'Unprotect' button and confirm transaction on the wallet
- Smart contract burns entered amount of urTokens and the respective crypto tokens will be transferred back into the user's wallet at 1:1 ratio
- When the transaction is confirmed onchain, the UI shows the amount of urTokens burned and the amount of crypto tokens received
- UI provides the user with a hyperlink for the user to review the transaction details on the block explorer 
- If the user protected their crypto tokens, then the user can unprotect (claim) their tokens at any time (without restrictions) using their Sign Key or Master Key


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

When these steps are applied and the user can see the field 'Reset Sign Key' to input and confirm new Sign Key, that means the Master Key has been transcribed without any misspellings and the user can allocate funds with 100% confidence into the contract, being assertive that in the event of losing/forgetting their Sign Key, they can input their Master Key and reset the Sign Key.

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

