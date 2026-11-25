# Nexora Privacy Policy

**Effective Date:** November 25, 2026  
**Contact Email:** `kungojo003@gmail.com`

## 1. Overview

Nexora is a private personal and household file-storage interface that lets invited household members connect and manage their own storage accounts through a single interface while keeping each person's cloud storage strictly isolated.

## 2. Google API Scope Used

Nexora requests only the following Google Drive OAuth 2.0 scope:

- `https://www.googleapis.com/auth/drive.file`

This per-file scope grants Nexora access solely to files and folders that Nexora itself creates or that the user explicitly selects/opens within Nexora. Nexora does **not** request broad read or full-drive scopes over your existing unrelated Google Drive files.

## 3. Data We Access & How We Handle It

- **Encrypted OAuth Credentials:** OAuth access tokens and refresh tokens are encrypted at rest on the server and are never stored in browser `localStorage`, `sessionStorage`, cookies, or unauthenticated API responses.
- **No Persistent Caching of Drive File Bytes:** Uploaded and downloaded Drive files are streamed directly between the authorized client session and Google Drive API v3 (`Cache-Control: no-store, private` on downloads). Nexora does not maintain a persistent copy or cache of your Google Drive file contents.
- **Metadata-Only Synchronization:** To display file listings and keep folder state accurate, Nexora stores only minimal catalog metadata for Nexora-managed files (such as Drive file ID, logical filename, file size, SHA-256 checksum, timestamps, and incremental Drive `changes` page tokens).
- **Strict Account & User Isolation:** Connected Google Drive accounts (`personal_cloud`) belong strictly to their connecting user. Nexora does not pool, shard, or cross-share Google Drive accounts between different users unless explicitly enabled by an administrator for a specific account.
- **No Selling, Advertising, or Third-Party Sharing:** Nexora does not sell, rent, trade, or transfer Google user data to third parties or advertisers.
- **No AI/ML Model Training or AI-Agent Access:** Google Drive content and metadata accessed through Nexora are never used to train, fine-tune, or evaluate AI/ML models, and Google Drive (`personal_cloud`) accounts and files are blocked by policy from AI agent/MCP access.

## 4. Google API Services User Data Policy (Limited Use)

Nexora's use and transfer to any other app of information received from Google APIs will adhere to the [Google API Services User Data Policy](https://developers.google.com/terms/api-services-user-data-policy), including the Limited Use requirements.

## 5. User Control, Revocation & Deletion

- **Immediate Disconnect & OAuth Revocation:** You may disconnect a Google Drive account at any time in Nexora, which revokes OAuth tokens upstream via Google's revocation endpoint and wipes stored credentials locally. You can also revoke Nexora's access at any time via your [Google Account Permissions](https://myaccount.google.com/permissions) page.
- **Metadata Deletion Requests:** To request permanent deletion of all associated user and catalog metadata, email `kungojo003@gmail.com`.

## 6. Changes & Contact

If this Privacy Policy is updated, the revised version will be posted here with an updated effective date. For any questions or data requests, contact `kungojo003@gmail.com`.
