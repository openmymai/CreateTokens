#### Create Token with the Token Program
- You may recall SOL is the 'native token' of Solana. All other tokens, fungible and non-fungible tokens (NFTs), are called SPL Tokens.
- The Token Program contains instructions for creating and interacting with SPL Tokens.
- Token Mints are accounts that define a specific token. This includes information about the token itself (like how many decimals it has), the account allowed to mint more tokens (called the mint authority), and where to find more information about the token like a description, image, etc. The mint authority can use the token mint to make more tokens!
- Token Accounts hold tokens of a specific Token Mint. For most users, their balances of each token mint are stored in Associated Token Accounts - accounts with addresses made from their wallet address and the token's mint.
- Creating Token Mints and Token Accounts requires allocating rent in SOL. The rent for a Token Account can be refunded when the account is closed. Additionally, tokens created with the Token Extensions Program can also close Token Mints.
