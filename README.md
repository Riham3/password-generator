# Riham Blogs' Password Generator
Generate secure passwords in bulk with simple to advanced customisation. No Sign-Up required. Privacy-focused.

Try it out at: [https://cigarettesprettysmokes.pages.dev/password/](https://cigarettesprettysmokes.pages.dev/password/)

## Overview
It uses the Web Crypto API for randomness, paired with Dropbox's zxcvbn (self-hosted) for password strength estimation.

Start by selecting one of the three modes ("Random", "Memorable", "Pattern"). The "bulk" input lets you generate more than one password in a single click.

Click on any password text to copy it directly from the table. Strength is indicated by a 0-4 score next to the password (e.g. "Passw0rd (0)").

| Score | Strength |
|-------|----------|
| 0 | Very weak |
| 1 | Weak |
| 2 | Fair |
| 3 | Good |
| 4 | Strong |

### Random
Generate a password of given length with characters from the selected charset(s) (e.g. "Ze&JNfkSi6dp4bL?").

### Memorable
Generate a password of given number of words from a list of ~360 English words by default (e.g. "Lunar3+Boldly2+Merely4").

It's possible to provide a list of custom words that you may want to use exclusively.

Use a custom separator, choose to capitalise the first letter of each word, and/or insert a randomized single digit at end of each word.

### Pattern
Generate a password based on a custom pattern using the tokens listed (e.g. "[A][a][0][*]" can generate a password like "Gx9!").

Use backslash (\\) before square or curly brackets to escape them as literal characters (e.g. "[0]\\{Ab\\}" can generate a password like "2{Ab}").

It uses the same set of words that are used by the "Memorable" mode for its word-based tokens (e.g. "{Ab}"), whether using the default list or your own custom words.

| Token | Meaning |
|-------|---------|
| [A] | Capital letter (A-Z) |
| [a] | Small letter (a-z) |
| [0] | Digit (0-9) |
| [*] | Symbol (e.g. !, @, #, $, %, etc.) |
| [?] | Any of the four above (A-Z, a-z, 0-9, etc.) |
| {Ab} | Word (first letter uppercase, rest lowercase e.g. Password) |
| {ab} | Word (all lowercase e.g. password) |
| {AB} | Word (all uppercase e.g. PASSWORD) |

## Privacy Notice
Everything runs locally, every generated password is temporarily stored in the DOM so closing (or refreshing) the tab permanently removes them.

It's also possible to use the app without an internet connection after you open the page as long as you don't refresh or navigate away from it.

## Feedback
Submit bug reports or request for features at: [https://cigarettesprettysmokes.pages.dev/feedback/](https://cigarettesprettysmokes.pages.dev/feedback/)

© 2026 Riham S. README content licensed under [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/). Last updated: 17.08.26
