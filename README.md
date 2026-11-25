# Nexora

Nexora is a private personal and household storage management interface designed to help authorized family and household members organize, upload, and access their own files cleanly while keeping personal cloud accounts strictly isolated.

## How Nexora Works with Google Drive

- **App-Scoped Permission Only (`drive.file`):** Nexora requests only the narrow `https://www.googleapis.com/auth/drive.file` OAuth scope, limiting access strictly to files created by or explicitly opened through Nexora. It cannot browse or modify unrelated files already stored in your Google Drive.
- **Private Per-User Isolation:** Each connected Google Drive account remains dedicated to its owning user. Nexora never pools, stripes, or merges personal Google Drive accounts across users.
- **No Persistent Content Caching or AI Training:** File bytes stream on demand without persistent server-side caching of Drive file contents (`Cache-Control: no-store, private`). Google Drive data is never used for AI/ML model training and is never exposed to AI agent tools.
- **Instant Disconnect & Revocation:** Any user can disconnect their Google Drive account from Nexora or revoke access at any time from their Google Account security settings.

## Privacy Policy

See [PRIVACY.md](./PRIVACY.md) for the full Privacy Policy and Google API Services User Data Policy (Limited Use) disclosures.

## Contact

For questions, account removal, or privacy inquiries, contact: `kungojo003@gmail.com`.
