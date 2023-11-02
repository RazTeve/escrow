**Questions to be answered:**

What's a PSBT?
A PSBT is a Partially Signed Bitcoin Transaction. It is a format for transactions that are not fully signed and allows for transactions to be passed around multiple parties until all necessary signatures are collected. Its purpose is to standardize the way different wallets and services handle the signing of transactions, especially in situations where multiple signatures are required, such as with multi-signature wallets. It enhances the flexibility and security of Bitcoin transactions.

Where does this fit in?
For Resolvr Escrow, both the bounty maker and taker would be required to agree on bounty terms and sign a PSBT broadcast by our service

How will escrow help me resolve disputes?


Hosted where?
Some microserver(rocket) somewhere until self-hosted 

Why use this stack?

What are DLCs/oracle/fedimint?

Why DLC instead of multisig escrow?
With 2:3 multisig the dispute resolution service could be considered to be a custodian, which presents legal risk. Using a DLC removes the liability created by joint-custody model.

Using DLC protects privacy by decoupling the dispute resolution service from the contracts its helps resolve. 

In the future DLCs can be lifted off chain onto lightning allowing users to save on fees. ^alreadypossible

Couldn't the oracle be compromised?
By using a federated signing process, frost, we remove a single point of failure.
A fedimint allows us to act as a singular entity.
