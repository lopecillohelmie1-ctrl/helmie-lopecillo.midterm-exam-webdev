# HelmieCramJam

HelmieCramJam is a lightweight, privacy-minded social media **frontend prototype** made with HTML, CSS, and Vanilla JavaScript. It is designed as a realistic multi-page demo for learning and presentation purposes.

## What is included?

- Home feed with sample posts, post creation, likes, and bookmarks
- Login and signup demo forms
- Profile page with editable display name and bio
- Explore page with search and topic shortcuts
- Bookmarks page for saved posts
- About page describing the project goals
- Privacy Center explaining local storage and allowing users to clear demo data
- Responsive layout for desktop and mobile screens

## Project structure

```text
HelmieCramJam/
├── index.html                 # Home feed and post composer
├── pages/
│   ├── login.html             # Demo login form
│   ├── signup.html            # Create a local demo profile
│   ├── profile.html           # View/edit profile and own posts
│   ├── explore.html           # Search posts and topics
│   ├── bookmarks.html         # Saved posts
│   ├── about.html             # Project purpose and principles
│   └── privacy.html           # Data notes and clear-data control
├── src/
│   ├── css/style.css          # Shared styling and responsive rules
│   └── js/main.js             # Feed, profile, search, likes, bookmarks
├── assets/                    # Reserved for local images/icons
└── README.md                  # Project documentation
```

## How to run

1. Download and extract the project ZIP.
2. Open the `HelmieCramJam` folder in Visual Studio Code or another editor.
3. Open `index.html` in a modern browser. For a smoother development workflow, use a local preview extension such as Live Server.
4. Visit the other pages using the navigation.

No build step, package installation, backend, database, or API is required.

## How it works

- The pages share one stylesheet (`src/css/style.css`) and one JavaScript file (`src/js/main.js`).
- Sample posts are provided in JavaScript and are shown until the user creates their own local feed data.
- Posts, profile details, liked post IDs, and bookmarks use the browser's `localStorage`.
- Signup and login are demonstrations. Login does **not** validate a password or create a secure session.
- The Privacy Center includes a control to remove this app's local demo data from the current browser.

## Privacy and security limitations

This is a static frontend prototype, not a secure social network. Browser `localStorage` is not encrypted and may be visible to someone with access to the same browser profile or device. There is no server-side authentication, authorization, encryption, moderation, backups, or cross-device syncing. Do not use real passwords or enter sensitive personal information. A production application would require a carefully designed backend, security review, and clear privacy policy.

The stylesheet imports Google Fonts for typography. To remove this external font request, delete the `@import` line at the top of `src/css/style.css`; the page will fall back to system fonts.

## Main interactions to test

1. Write and publish a post on the home page.
2. Like and bookmark posts, then check the Bookmarks page.
3. Search for words such as `privacy`, `technology`, or `creativity` on Explore.
4. Open My Profile and edit the display name or bio.
5. Open the Privacy Center and clear local demo data if needed.

## Suggested improvements

- Add keyboard-focused accessibility checks and more automated testing.
- Add moderation/reporting UI for a fuller prototype.
- If a backend is ever introduced, implement real authentication, access controls, secure transport, data deletion, and privacy review before using real user data.

## License

This educational prototype is provided for learning and customization. Add an explicit license if you publish or redistribute it.
