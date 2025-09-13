# DATA_USAGE.md
- ***DATA COLLECTION IS CURRENTLY DISABLED, AS THIS FEATURE IS NOT FULLY DEVELOPED.***
- ***USERS WILL BE NOTIFIED BEFORE ANY DATA IS COLLECTED.***
- ***This file will most likely be changed frequently!***
  
## Data Usage & Privacy (AutoPrimaryPart / APP)

**Last updated:** 2025-09-12  
**Version:** v0.1.0-beta


### Summary
APP collects only minimal technical identifiers and statistics necessary for its functionality. All data is used exclusively for feature management, moderation, and error diagnosis. Users can control or disable data collection via plugin settings, and sensitive personal information is never stored.

---

## What APP collects

### Identifiers
- **SeemBuilds_User_ID** —  An internal identifier for overall control over SeemBuilds plugin users. Nothing about the user and their roblox place is stored here, only plugin statistics such as total downloads, but also access rights for certain plugins.
- **APP_User_ID** — an internal identifier assigned to the user for tracking feature access and usage, specifically for APP. 
- **SeemBuilds_Token_ID** — a token used for server-side validation (never stored in client-readable plaintext).

These identifiers are used only for technical identification and internal logic. They do **not** identify personal details outside the system.

### Usage & Debugging Data
When reporting is enabled, APP may collect technical details to support debugging or error resolution:
- Model metadata related to the operation that triggered an error (e.g., part counts, bounding box dimensions, part volumes, relevant PrimaryPart properties).  
- APP plugin state information at the time of the operation (active mode, relevant settings).  
- Timestamps and the APP_User_ID (or anonymized ID if anonymous mode is enabled).

**Important:** Model names, project names, personal names, and project files are **never** collected. Only statistical/technical values are used for debugging or analytics.

---

## Purpose of Collection

- **Feature Flags / Selective Rollout:** to enable specific features for selected users, such as beta testing or staged rollouts.  
- **Moderation & Bans:** to restrict plugin usage in abusive contexts. (APP cannot independently determine malicious activity; bans rely on heuristic checks and manual review.)  
- **Debugging & Quality Improvements:** minimal technical details allow reproduction and correction of errors, improving stability and functionality.

---

## Data Storage

- **Feature flags & user identifiers:** stored in Firebase Realtime Database or another configured server-side store.  
- **Debugging / event messages:** sent via webhook to a private Discord server (controlled by the developer only) and are **not** stored in Firebase.  
- **Tokens & secrets:** stored only in server-side environment variables or secret managers. APP does **not** embed long-lived secrets in client code.

---

## Security Considerations

- Use HTTPS for all communication.  
- Protect Firebase rules to prevent unauthorized reading or writing.  
- Treat Discord webhooks as private; rotate if compromised.  
- Tokens are stored server-side and never exposed to clients.

---

## Controls & Opt-Out

APP provides options for controlling data collection:

- **Anonymous Mode / Minimal Mode:** sends only aggregated or anonymized statistical values.  
- **Telemetry Off:** disables all usage & error reporting.  
- **Manual Debug Log:** sends debugging info only when explicitly triggered by the user.

---

## Data Retention & Deletion

- Debug messages in Discord can be deleted manually by the server owner.  
- Firebase records (feature flags, minimal user records) are retained until a deletion request is received.  
- Deletion requests can be submitted via GitHub Issues or email, providing the APP_User_ID for identification.

---

## Moderation & Bans

- Bans may be applied to APP_User_IDs to restrict access to certain features or updates.  
- APP cannot fully determine malicious intent on its own; bans are applied conservatively.  
- Appeals can be submitted through GitHub Issues or email.

---

## Legal / GDPR Disclaimer

This document is for informational purposes and does not constitute legal advice. Users in regions with data protection laws (e.g., GDPR/DSGVO) should consult appropriate legal guidance.
