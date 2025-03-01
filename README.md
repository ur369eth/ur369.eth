# urToken (Ultra Resistant Tokens) - Function wise functionality is described in Code.

Description of working of Smart Contract is as follows:

## Functionalities

- Decentralized Protection (lock) of Native Tokens / Mint of urTokens
- Transfer urTokens
- Unlocking Native Tokens
- Fee Collection System (Benefaction-fee)
- Award System
- Whitelist Mechanism
- Master Key and Sign Key (or Quantum Key) Mechanism to perform any action
- Quantum Resistan Approach

### Decentralized Protection of Native Tokens / Mint of urTokens:

**_Definition:_** The decentralized protection of native tokens from theft and quantum threats occurs by (A) removing native tokens from circulation, safeguarding them within the smart contract and by (B) minting urTokens, issued at 1:1 ratio in regards of the protected native tokens. The smart contract delivers urTokens to the user and the urTokens can only be transfered with a Sign Key.

Example: end-user protects 10 GHO, and the smart contract automatically displays a benefaction-fee of 0.369% (the benefaction-fee is shown upfront to the user to exert full transparency and for the user to become aware of it); the benefaction-fee is used to fund public goods and other important causes, randomly award end-users, contribute to the comunity, developers and to sustain ur369.eth (the social good).

10 GHO - 0.369% = 9.9631 GHO; thus the ur369 smart contract mints 9.9631 urGHO (ultra resistant GHO) into end-user's account. With a click of a button the user can add the minted urTokens to their wallet.

**_Procedure_**

- Enter desired amount to be protected (isolated away from circulation).
- The System will check if end-user is new to the system or not. In case of new user, the system will provide a Concealed Master Key.
- The system prompts the end-user to set and confirm a Sign Key (i.e., a strong password or PIN).
- User has the option to set and confirm a quantum resistant Sign Key (instead of classical Sign Key).
- End-user signs an on-chain transaction to set and confirm Sign Key (or quatum resistant Sign Key).
- Upon the on-chain transaction confirmation, the smart contract will save user's Sign Key (or quantum resistant Sign Key) and Master Key.
- At this point the user/address is registered in the system and the system prompts the user with the form to input the desired amount of native tokens to protect.
- After the user inputs the amount of native tokens to protect, the system automatically displays the 0.369% benefaction-fee and shows the user the amount of urTokens that user will receive.
- If all ok for the user they can proceed with their operation to protect (lock) native tokens and mint urTokens.
- The user can use the ur369.eth interface any time and will use the Sign Key (or quantum resistant Sign key) to perform the operations: Protect (i.e., lock/safeguard native token(s) and mint urToken(s) to themselves). Transfer (i.e., send urToken(s)). Claim (i.e., burn urToken(s) to unlock/unprotect native tokens).
- The Master Key helps the end-user to reset their Sign Key (in case Sign Key is lost).

Note: The Master Key is randomly generated on-chain and encrypted. It will be presented only once and must be kept someplace safe (preferably offline). The Master Key is issued with separators (-) to facilitate its migration from online to off-line with near-zero chances of mispelling it. 

The system indicates the step-by-step instructions to the user in order to ***safely transcribe*** the Master Key from online to offline.
A state-of-the-art OpSec can be seen in ur369.eth.limo >> tab "Insight", point (23).

### Transferring urTokens

**_Description:_** urTokens can only be transfered if-and-only-if the end-user enters their Sign Key.

- Click on "Transfer" button for the respective urToken to populate the transfer form (pop-up/modal).
- Enter amount and recipient address.
- Enter Sign Key (or quantum resistant Sign key) and click on "Transfer" button.
- Confirm transaction in wallet.
- Smart contract will transfer urTokens from sender to recipient.
- The recipient(s) of urTokens can use the decentralized u369.eth interface at any time to transfer their urTokens and/or to claim native tokens.

### Unlocking/unprotecting Native Tokens

**_Definition:_** Unlocking/unprotecting native tokens from within the contract to receive native tokens back into your wallet. 

Example: end-user wants to claim the locked/protected 9.9631 GHO; then user must burn 9.9631 urGHO, they will enter 9.9631 urGHO and the smart contract will burn the 9.9631 urGHO and return 9.9631 GHO to the end-user's wallet.

**_Procedure_**

- Enter desired amount of urTokens to burn in order to unlock/unprotect the respective amount of native tokens.
- Input Sign key (or quantum resistant Sign key) and click "Unprotect" button.
- Confirm transaction in your wallet.
- Smart contract will burn amount of respective urTokens from account of user.
- Respective native tokens will be transferred back to the user's wallet.

### Fee Collection System

**_Description:_** Each time an end-user protects (locks) native tokens, a specific and fix percentage (0.369%) will be shown to the user before the operation takes place. If user is ok with the service (benefaction-fee), then the 0.369% is automatically deducted from the entered amount and the remaining amount will be safeguarded (locked) within the contract.

**_0.369% Benefaction Fee Automatic Collectors_**

The contract programmatically distributes the collected benefaction fee in order to serve a purpose of social impact and sustainable contribution (social good) to the ecosystem.

1. 30% of 0.369% will be transferred to urgift.eth to reward a randomly selected user every 369 hours.
2. 30% of 0.369% will be transferred to ur-impact.eth to fund public goods and other important causes.
3. 30% of 0.369% will be transferred to ur369.eth address to self sustain ur369.eth the social good.
4. 10% of 0.369% will be transferred to ur369community-devs.eth for the ur369 Community & Developers Benefit Fund.

   **_Procedure_**

- Benefaction-fee will be deducted at the time of protecting (locking) native tokens (which is also automatically minting urTokens).

### Award System (Timeless Pools)

**_Description:_** Upon start of each time period, a user will be randomly selected to receive all or part of the award collected in previous non-collected time periods.

There are 3 Timeless Pools. The Gift Pool, The Impact Pool and the Stateless Pool.

Two of them (the Gift Pool and the Stateless Pool) use the following formula to randomly select the "Recipient" candidate:

uint randomNumber = uint(keccak256 (abi.encodePacked (previousTimePeriod, deployTime))) % depositorsLength;

In simple words, the procedure is defined in the following steps:

1. A keccak hash (hashing algorithm) is applied on the previous time period and contract deploy time.
2. Hash is converted to integer value.
3. A modulus operation performs on the converted integer and number of addresses in the last time period.

(A) Gift Pool

Description: Every 369 hours a "Recipient" candidate will be randomly selected. The candidate can receive the full amount within the pool if the proper pool's stated conditions are met.

**_Procedure_**

- Each detail will be shown on the "Awards" page regarding collectable assets.
The randomly selected "Recipient" candidate's address (6 first and 6 last carachters) will be shown in the "Awards" page.

- If the "Recipient" candidate fulfils the Gift Pool's stated conditions, the award will be sent from the urgift.eth address to the randomly selected "Recipient" candidate's address. The "Recipient" candidate has 3 days, 6 hours and 9 minutes to fulfill their part after being selected. If fulfilled the "Recipient" candidate will receive their award within within the next 3 days, 6 hours and 9 minutes.

Gift Pool Conditions can be seen in the ur369.eth UI (Awards page). These conditions are outside of the code's scope as those are bound to a game theoretical approach and are performed manually (purpose of executing it manually is to avoid a sybil exploit that can happen when delivering the award(s) programatically).

(B) The Impact Pool (ur-impact.eth) is modular pool and it is a supplementary receiver of funds, it does not have its own timer per se; however, it works in parallel with the 369 hours timer. Funds within this pool are used to fund public goods and other important causes, to boost the awards for users if certain criteria is met, to award anyone that contributes with a meanigful idea and their idea is (or will be) implemented.

(C) Stateless Pool

Description: A "Recipient" candidate is randomly selected every 369 days.

**_Procedure_**

The random selection every 369 days works within the same conditions as the random selection every 369 hours. Please see "Awards" page >> Stateless Pool Conditions.

Note: After the award is sent to the randomly selected "Recipient" candidate, any remaining funds within the Stateless Pool address will flow to the ur369fractal.eth smart contract to be distributed as follows:

10% to the ur369 Community & Developers Benefit Fund
30% to fund public goods and other important causes
30% to randomly award the end-users
30% to u369.eth (the social good)

### Whitelist Mechanism

**Definition:** For the whitelisted smart contract addresses, the users don't need to enter Sign Key (or quantum resistant Sign key) for the transferring of funds (urTokens).

**Implementation Guide:**

Whitelisted smart contract address can be, for example Uniswap, v4 (whitelisted), AAVE v3 and other DeFi platforms (to be whitelisted in the future):
The system will check if the sender is a whitelisted contract address, and then the system will allow the whitelisted contract to transfer urTokens without any Sign Key.

**Strategy to Implement Whitelist Functinality:**
There are two ways to check that caller is a contract address or not:

- if(msg.sender == tx.origin): in case of true, caller is EOA otherwise caller is a contract.
- if(msg.sender.code.length == 0): in case of true, caller is an EOA otherwise caller is a contract.
- **_Note:_**
1. Any of above can be used to check whether caller is an EOA or a contract.
2. isContract() function of Address Library is deprecated due to security reasons.

### Master Key and Sign Key (or Quantum Key) Mechanism to perform any action

**_Description:_** To prevent users from transferring funds directly from any wallet, the system implements this feature. On each urTokens operation (protect, transfsr or claim/unprotect). the user must enter their Sign Key on the ur369.eth.limo UI otherwise transaction will fail.

In case of losing or forgetting Sign key, a recovery phrase functionality mechanism is implemented:

If end-user wants/has to change their Sign Key, the Master Key will be used.

### Quantum Resistant Approach

**_Overview:_** With the advancements in quantum computing, traditional cryptographic approaches are becoming increasingly vulnerable. To future-proof the ecosystem, the Dilithium-Crystals quantum-resistant algorithm is used.

**_Implementation Flow:_** 

**(A) Hashing with Keccak-256:** First the Master Key and the Sign Key are hashed with Keccak-256, a reliable algorithm widely used in blockchain, to add another layer of security.

**(B) Applying Quantum-Resistant Signature (Dilithium-Crystals):** Upon enabling the Master Key and Sign Key, a Dilithium-Crystals signature is generated, ensuring a high level of quantum security. This signature, together with the public key, is stored on the blockchain, creating a secure reference point for future verification.

**(C) Signing with the crypto wallet Private Key:** The Keccak-256 hash is signed using the user’s wallet private keys, which authenticates the transaction on the blockchain and adds an extra verification layer.

**(D) Storing Data on Blockchain:** The Dilithium-Crystals signature, public key, Keccak-256 hash, and the wallet signature are securely stored on the blockchain. To ensure authenticity, the Wallet signature is verified using the ecrecover function, validating the signature against the user’s address.

**(E) Sign Verification Process:** To sign, the user enters their Sign key, and the Keccak-256 hash is regenerated. This hash is then compared against the stored data on the blockchain. A new Wallet signature is created and verified on-chain.

**(F) Rationale for selecting Dilithium-Crystals among other NIST-recommended algorithms:** NIST recommends multiple quantum-resistant algorithms, (e.g., SPHINCS+, Rainbow, Dilithium-Crystals, etc.) -- Dilithium-Crystals offers efficient storage, consistent key generation, and resilient security against both classical and quantum attacks.

**_Multi-Layered Security:_** 

**Front-End Quantum-Resistant Signature:** Dilithium-Crystals applied on the front end ensures protection against quantum threats.

**Backend Keccak Hash:** The Keccak-256 hash provides backend-level protection, safeguarding the Master Key and the Sign Key on-chain.

**Frontend-Backend Connection Verification:** Works for both Classic and Quantum Protection, thus by requiring the Sign Key and/or the Quantum Resistant Sign Key (when enabled) to sign >> unauthorized direct access is prevented, ensuring that only onchain-verified-users can interact with the application.

Note: Onchain-verified users does not relate nor indicates KYC (Know Your Customer); the onchain-verification, in this context, means the users having created their Sign Key and/or their Quantum Resistant Sign Key.
