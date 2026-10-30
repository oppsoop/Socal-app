# Mingle prototype

A small, original social-app prototype inspired by the requested experience (not a copy of K-Friends). Run with Node.js 22.5 or newer:

```sh
npm start
```

Open http://localhost:3000. Create two accounts in separate browser sessions to search for a unique username and exchange text messages. Data is stored in a local SQLite file (`socal.db`); set `DATA_FILE` to choose a different file path. Set `PORT` to change the port. This is a development prototype, **not production-ready**.

## Included

- Email/password signup and login, case-insensitively unique usernames and emails, server-side sessions, scrypt password hashes.
- Username search and one-to-one text messages, polled every five seconds.
- A responsive discovery interface and placeholders for future features.

## Important limitations

Google sign-in, email verification, password reset, calls, images/videos, live location, moderation tools, an administrator app, notifications, encryption in transit or end-to-end, account deletion, backups and auditing are **not implemented**. Messages are stored in plaintext in the local database and are accessible to whoever controls it. Do not use real personal information or deploy publicly. Passwords are hashed and cannot be viewed by administrators. Administrative access to private content should be transparent, access-controlled, justified, and audited; it must not expose passwords.

Before a real launch, the service needs HTTPS, a production database and secure storage, robust authentication and rate limiting, CSRF and abuse protection, authorization reviews, privacy and retention policies, user consent, blocking and reporting, moderation, age safeguards, independent security audits, legal review, and platform-specific compliance. No security audit or legal certification has been performed. Third-party remote photos and fonts are used in the prototype and should be replaced with licensed assets before launch. No license for K-Friends, its name, branding, or features is granted by this project.
