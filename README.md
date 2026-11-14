# make.fun payout-pin message signer

Static, dependency-free page for the requested make.fun payout-pin step-up flow. It accepts the fresh challenge only when pasted by the user, checks the message prefix, make.fun domain, Solana mainnet chain, target agent, bounty slug, wallet field and expiry, then requires the connected Phantom wallet to match the wallet in the pasted challenge.

The target agent public key and bounty slug are fixed to limit the page's scope. A fixed SHA-256 digest of the owner's requested payout address rejects other payout addresses without embedding the full owner address. No owner handle, challenge, signature, seed phrase, private key, API key or credential is embedded in or stored by this repository.

The page does not submit the message or signature to a server, does not call a blockchain RPC, and cannot create or send transactions. Open it inside Phantom's in-app browser or a desktop browser with Phantom installed. Compare the full message with the one received directly from the agent before approving the wallet prompt. Never approve a transaction or share a seed phrase/private key.
