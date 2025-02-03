# urToken (Ultra Resistant Tokens) - Function wise functionality is described in Code.

Description of working of Smart Contract is as follows:

## Functionalities

- Decentralized Lock of Native Tokens / Mint of urTokens
- Transfer urTokens
- Unlocking Native Tokens
- Fee Collection System (Benefaction-fee)
- Award System
- Whitelist Mechanism
- Concealed Master Key (Master Key) and Sign Key Mechanism to perform any action (plus Quantum Key option)

### Decentralized Lock of Native Tokens / Mint of urTokens:

**_Definition:_** Decentralized locking is protecting native tokens from theft and quantum threats by isolation (removing native tokens from circulation) and safeguarding them within the smart contract. 

Mint of urTokens is the issuance at 1:1 ratio in regards of the locked native tokens. The smart contract delivers urTokens to the user protecting/locking the native tokens.

Example: end-user protects/locks 10 GHO, and the smart contract automatically takes a benefaction-fee of 0.369% (the benefaction-fee is previously displayed to the user to exert full transparency and for the user to become aware of it) the benefaction-fee is used to fund public goods and other important vauses, award end-users, contribute to the comunity, developers and to sustain ur369.eth (the social good).

10 GHO - 0.369% = 9.9631 GHO; thus the ur369 smart contract mints 9.9631 urGHO (ultra resistant GHO) tokens into end-user's account and from the user interface they can add the minted urTokens to their wallet.

**_Procedure_**

- Enter desired amount to be locked/protected.
- The System will check if end-user is new to the system or not. In case of new user, the system will provide a Concealed master Key.
- The system prompts the end-user to set and confirm a Sign Key (i.e., a strong password or PIN).
- User has the option to set and confirm a quantum resistant Sign Key (instead of convetional Sign Key).
- End-user signs an on-chain transaction to set and confirm Sign Key (or quatum resistant Sign Key).
- Upon the on-chain transaction confirmation, the smart contract will save user Sign Key (or quantum resistant Sign Key) and Master Key.
- At this point the user/address is registered in the system and the system prompts the user with the form to input the desired amount of native tokens to protect.
- After the user inputs the amount of native tokens to protect, the system automatically displays the 0.369% benefaction-fee and shows the user the amount of urTokens that user will receive.
- If all ok for the user they can proceed with their operation to lock native tokens and mint urTokens.
- The user can use the ur369.eth interface any time and will use the Sign Key (or quantum resistant Sign key) to perform the operations: Protect (i.e., lock/safeguard native token(s) and mint urToken(s) to themselves). Transfer (i.e., send urToken(s)). Claim (i.e., burn urToken(s) to unlock/unprotect native tokens).
- The Master Key helps the end-user to reset their Sign Key (in case Sign Key is lost).

Note: The Master Key is randomly generated on-chain and encrypted. It will be presented only once and must be kept someplace safe (preferably offline). The Master Key is issued with separators (-) to facilitate its migration from online to off-line with near-zero chances of mispelling it. 

The system indicates to the user in order to safely transacribe the Master Key from online to offline with a state-of-the-art OpSec. See "Insight (23)".

### Transferring urTokens

**_Description:_** urTokens can only be transfered if-and-only-if the end-user enters their Sign Key.

- Click on "Transfer" button for the respective urToken to populate the transfer form (pop-up/modal).
- Enter amount and recipient address.
- Enter Sign Key (or quantum resistant Sign key) and click on "Transfer" button.
- Confirm transaction in wallet.
- Smart contract will transfer urTokens from sender to recipient.
- The recipient(s) of urTokens can use the permissionless and decentralized u369.eth interface at any time to transfer their urTokens and/or to claim native tokens.

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

**_Description:_** Each time an end-user locks/protects native tokens, a specific and fix percentage (0.369%) will be deducted from the entered amount and remaining amount will be locked/safeguarded.

**_0.369% Benefaction Fee Automatic Collectors_**

1. 30% of 0.369% will be transferred to urgift.eth to reward a randomly selected user every 369 hours.
2. 30% of 0.369% will be transferred to ur-impact.eth to fund public goods and other important causes.
3. 30% of 0.369% will be transferred to ur369.eth address to self sustain ur369.eth the social good.
4. 10% of 0.369% will be transferred to ur369community-devs.eth for the ur369 Community & Developers Benefit Fund.

   **_Procedure_**

- Benefaction-fee will be deducted at the time of locking/protecting native tokens (i.e., minting urTokens).

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

Description: Every 369 hours a "Recipient" candidate will be randomly selected. The candidate can receive the full amount of awards if the proper pool's stated conditions are met.

**_Procedure_**

- Each detail will be shown on the "Awards" page regarding collectable assets.
The randomly selected "Recipient" candidate's address (6 first and 6 last carachters) will be shown in the "Awards" page.

- If the "Recipient" candidate fulfils the Gift Pool's stated conditions, the award will be sent from the urgift.eth address to the randomly selected "Recipient" candidate's address. The "Recipient" candidate has 3 days, 6 hours and 9 minutes to fulfill their part after being selected. If fulfilled the "Recipient" candidate will receive their award within within the next 3 days, 6 hours and 9 minutes.

Gift Pool Conditions can be seen in the ur369.eth UI (Awards page). These conditions are outside of the code's scope as those are bound to a game theoretical approach and are performed manually.

(B) The Impact Pool (ur-impact.eth) is modular pool and is a supplementary receiver of funds, it does not have its own timer per se; however, it works in parallel with the 369 hours timer. Funds within this pool are used to fund public goods and other important causes, to boost the awards for users if certain criteria is met, to award anyone that contributes with a meanigful idea and their idea is (or will be) implemented.

(C) Stateless Pool

Description: A "Recipient" candidate is randomly selected every 369 days.

**_Procedure_**

The random selection every 369 days works within the same conditions as the random selection every 369 hours. Please see "Rewards" page >> Stateless Pool Conditions.
Note: After the award is sent to the randomly selected "Recipient" candidate, any remaining funds within the Stateless Pool address will flow to the ur369fractal.eth smart contract to be distributed as follows:

10% to the ur369 Community & Developers Benefit Fund
30% to fund public goods and other important causes
30% to randomly award the end-users
30% to u369.eth (the social good)

### Whitelist Mechanism

**Definition:** For the whitelisted smart contract addresses, the users don't need to enter Sign Key (or quantum resistant Sign key) to perform a transaction from UI for transferring funds.

**Implementation Guide:**

Whitelisted smart contract address is for example Uniswap v4 or AAVE v3:
The system will check if the sender is a whitelisted contract address, and then the system will allow the whitelisted contract to transfer urTokens without any Sign Key.

**Strategy to Implement Whitelist Functinality:**
There are two ways to check that caller is a contract address or not:

- if(msg.sender == tx.origin): in case of true, caller is EOA otherwise caller is a contract.
- if(msg.sender.code.length == 0): in case of true, caller is an EOA otherwise caller is a contract.
- **_Note:_**
  1. Any of above can be used to check whether caller is an EOA or a contract.
  2. isContract() function of Address Library is deprecated due to security reasons.

### Master Key and Sign Key (or quantum Key) Mechanism to perform any action

**_Description:_** To prevent users from transferring funds directly from any wallet, the system implements this feature. On each urTokens operation (protect, transfsr or claim/unprotect). the user must enter their Sign Key on the ur369.eth.limo UI otherwise transaction will fail.

In case of losing or forgetting Sign key, a recovery phrase functionality mechanism is implemented:

If end-user wants/has to change their Sign Key, the Master Key will be used.
