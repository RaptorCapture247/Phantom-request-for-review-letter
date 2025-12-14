I am also experiencing this exact behavior when using Phantom Wallet with Pond0x subscriptions.

I can confirm that initial subscriptions are allowed, renewals before expiration are allowed, and once a subscription tier expires, Phantom blocks re-subscription to that same tier. Switching to a different tier works until that tier expires, after which previously expired tiers remain blocked. The behavior appears tied to subscription expiration state per tier, not transaction safety.

All other Pond0x interactions continue to work normally for me, including wallet connection, swaps, and other signatures.

This appears to be a reproducible, state-based false positive rather than a malicious transaction. I’m adding my confirmation here to help demonstrate that this affects multiple users.
