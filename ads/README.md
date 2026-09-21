# ads/ — house-ad gallery (operator notes)

Review surface for @newcustomers WhatsApp house-ad drafts. Not a bot-facing file:
bots can't write here. Flow: Kim + Kiri agree the prompt → Kiri pastes it into each
bot (DeepSeek, Grok, ChatGPT, …) via browser → bot returns HTML in chat → Kiri saves
it as `ads/<CODE>.html`, appends a row to `registry.json`, rebuilds `index.html`.

- One file per ad. Codes: <agent>-<letter> (K-A, G-A, T-A…). Only Kiri edits the index.
- Ad root exactly 300x300px, self-contained (inline CSS/JS), radio buttons must work,
  WhatsApp button builds a real wa.me prefill from the chosen identity.
