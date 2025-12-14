False-Positive Transaction Blocking on Pond0x Subscription Renewals (Metavault Program)

Hello Phantom Support Team,

I am writing on behalf of myself and other users in the Pond0x community to bring attention to a consistent transaction-blocking issue we are experiencing in Phantom Wallet that appears to be a false positive.


---

Summary of the Issue

Pond0x (https://pond0x.com) offers a legitimate subscription model that allows users to upgrade to a “Pro” tier for enhanced participation perks. There are three subscription durations available:

1 Week (0.3 Sol)

1 Month (1 Sol)

1 Year (10 Sol)


Phantom Wallet allows all three subscriptions to be purchased and renewed successfully so long as  renewal occurs before the active subscription expires.

However, once a subscription expires, Phantom Wallet blocks attempts to re-subscribe to that same tier, even though the transaction structure, program, and destination wallet remain unchanged.


---

Additional Observed Behavior (Tier Switching)

An important pattern we have observed:

If a user allows the 1-month tier to expire, Phantom blocks renewal of the 1-month tier

The user can still successfully subscribe to a different tier (1-week or 1-year)

Renewals for the new tier succeed as long as they occur before expiration

If the second tier is later allowed to expire, Phantom then blocks both expired tiers

The remaining unused tier continues to work

This process repeats until all tiers have expired, at which point all subscription tiers are blocked


This behavior suggests the blocking is tied to subscription expiration state per tier, rather than to transaction risk or malicious activity.


---

Relevant On-Chain Programs and Accounts

The subscription system uses a Pond0x-specific Metavault implementation on Solana. While this program is new and distinct to Pond0x, it is transparent, on-chain, and fully reviewable.

Metavault Program (Solana)

Program Account:
BgjbScBfUtSnP6JoPvnFRVDvqmcfByygz8GQjLjeNqgV

Solscan:
https://solscan.io/account/BgjbScBfUtSnP6JoPvnFRVDvqmcfByygz8GQjLjeNqgV

What are Metavaults:
https://www.hwonder.com/posts/metavault

Metavault Designer:
https://github.com/hWonderOfTheWorld

---

Subscription Payment Destination Wallet

Account:
GSMBLYht4JGmm1ZofyTFTGykYCwsenNQpRmiJ5fMnHpD

Solscan:
https://solscan.io/account/GSMBLYht4JGmm1ZofyTFTGykYCwsenNQpRmiJ5fMnHpD


---

Evidence of Safe and Allowed Interactions

Phantom Wallet successfully allows the following Pond0x interactions without issue:

Connecting a wallet to Pond0x

Swaps

Xminer connection signatures

Wallet cleaner actions

Initial subscription purchases and pre-expiration renewals


Only post-expiration renewals of previously used tiers are blocked.


---

Transaction History References

Below are Solscan links to previous successful subscription transactions for reference:

[PASTE SOLSCAN LINK HERE]

[PASTE SOLSCAN LINK HERE]

[PASTE SOLSCAN LINK HERE]



---

Request for Review

Given that:

The program and destination wallet are unchanged

Identical transactions succeed under specific timing conditions

Blocking occurs only after a tier expires

All other Pond0x transactions are permitted


We believe this is an automated policy or heuristic edge case rather than a genuine security concern.

We respectfully request that Phantom:

1. Review this specific Metavault subscription transaction pattern


2. Clarify why subscription expiration state affects approval


3. Adjust or whitelist this behavior if appropriate



This issue directly impacts legitimate users and creates unnecessary friction for a growing and potentially revolutionary onchain economy program.

Thank you for your time and consideration.

Kind regards,
[Your Name]
Pond0x Community Member
[Optional: Wallet Address]
Renewals for the new tier succeed as long as they occur before expiration

If the second tier is later allowed to expire, Phantom then blocks both expired tiers

The remaining unused tier continues to work

This process repeats until all tiers have expired, at which point all subscription tiers are blocked


This behavior suggests the blocking is tied to subscription expiration state per tier, rather than to transaction risk or malicious activity.


---

Relevant On-Chain Programs and Accounts

The subscription system uses a Pond0x-specific Metavault implementation on Solana. While this program is new and distinct to Pond0x, it is transparent, on-chain, and fully reviewable.

Metavault Program (Solana)

Program Account:
BgjbScBfUtSnP6JoPvnFRVDvqmcfByygz8GQjLjeNqgV

Solscan:
https://solscan.io/account/BgjbScBfUtSnP6JoPvnFRVDvqmcfByygz8GQjLjeNqgV

What are Metavaults:
https://www.hwonder.com/posts/metavault

Metavault Designer:
https://github.com/hWonderOfTheWorld

---

Subscription Payment Destination Wallet

Account:
GSMBLYht4JGmm1ZofyTFTGykYCwsenNQpRmiJ5fMnHpD

Solscan:
https://solscan.io/account/GSMBLYht4JGmm1ZofyTFTGykYCwsenNQpRmiJ5fMnHpD


---

Evidence of Safe and Allowed Interactions

Phantom Wallet successfully allows the following Pond0x interactions without issue:

Connecting a wallet to Pond0x

Swaps

Xminer connection signatures

Wallet cleaner actions

Initial subscription purchases and pre-expiration renewals


Only post-expiration renewals of previously used tiers are blocked.


---

Transaction History References

Below are Solscan links to previous successful subscription transactions for reference:

[PASTE SOLSCAN LINK HERE]

[PASTE SOLSCAN LINK HERE]

[PASTE SOLSCAN LINK HERE]



---

Request for Review

Given that:

The program and destination wallet are unchanged

Identical transactions succeed under specific timing conditions

Blocking occurs only after a tier expires

All other Pond0x transactions are permitted


We believe this is an automated policy or heuristic edge case rather than a genuine security concern.

We respectfully request that Phantom:

1. Review this specific Metavault subscription transaction pattern


2. Clarify why subscription expiration state affects approval


3. Adjust or whitelist this behavior if appropriate



This issue directly impacts legitimate users and creates unnecessary friction for a legitimate onchain economy.

Thank you for your time and consideration.

Kind regards,
[Your Name]
Pond0x Community Member
[Optional: Wallet Address]
