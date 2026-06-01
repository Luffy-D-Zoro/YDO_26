# Contributing to YDO

Hello contributors both new and old! Please read the following guidelines before contributing.

---

## Setting up locally
Please refer to the **[SETUP.md](docs/SETUP.md)** for instructions on setting up the project locally.

---

## Your First Code Contribution

Follow this general workflow for code contributions:

```bash
# Fork the repository and clone your fork
git clone [your-fork-url]

# Create a new branch
git checkout -b feature/your-feature-name
# or
git checkout -b bugfix/issue-description

# Make your changes

# Commit your changes following our commit message guidelines

# Push your branch
git push origin feature/your-feature-name
```

Then, open a Pull Request (PR) to the `main` branch. Provide a clear description and reference related issues.

---

## Commit Message Guidelines

We use **Conventional Commits**. Our Commitlint configuration enforces the following format:

```
<type>(<scope>): <subject>

<body>

<footer>
```

**Rules Explained:**

* **`<type>` (Mandatory):** Must be one of the following (lower-case):

  * `build`: Build system or external dependencies

  * `chore`: Routine tasks (e.g., updating dependencies)

  * `ci`: CI configuration changes

  * `docs`: Documentation-only changes

  * `feat`: New feature

  * `fix`: Bug fix

  * `perf`: Performance improvements

  * `refactor`: Code restructuring without behavior change

  * `revert`: Reverting a previous commit

  * `style`: Code formatting, white-space, etc.

  * `test`: Adding/correcting tests

* **`<scope>` (Optional):** Short description of the scope (e.g., `frontend`, `backend-auth`).

* **`<subject>` (Mandatory):** Concise description of the change:

  * Use imperative, present tense (e.g., add not added)

  * No capitalization at the beginning

  * No period (.) at the end

  * Max 100 characters

* **`<body>` (Optional):** Longer description of the commit:

  * Start with a blank line after subject

  * Describe what and why

  * Max line length: 100 characters


* **`<footer>` (Optional):** Information like breaking changes or issue references:

  * Start with a blank line after body

  * Reference issues (e.g., `Closes #123`, `Fixes #456`)

**✅ Example Commit Message:**

```
feat(frontend): add responsive navigation bar

This commit introduces a new responsive navigation bar for better user experience on mobile devices.

Closes #789
```

To perform multiline commit message you could use `git commmit` and then write the message in your editor.

---

## Development Workflow

1. Frontend
  * Landing Page
  * Login/Registration Page
  * A page showing the 12 word seed phrase with a feature to auto download the text file.
  * A Page to enter the first three letters of the seed phrase to verify the user.
  * A page to setup a 4 word pin.
  * Dashboard Layout.
  * Search Layout.
  * Countdown page.
  * Match Reveal Screen.
  
2. Backend
  * Configure Supabase to reject all non *iiitdmj.ac.in domains.
  * Pre-populate the database with all college roll numbers to serve as public directory.
  * Implement a database rule that automatically rejects any new submissions after the deadline.  
  * Write the Match Aggregation script to scan the database and group all mutual matches (hashes appearing exactly twice).  
  * Setup the automated export of the matched hashes into a lightweight .json file. 

3. Core Logic
  * Implement mnemonic and keypair generation using ether.js
  * Implement AES_GCM encryption to secure the 12 word phrase into the browser local storage.
  * Implement the Elliptic Curve Diffie-Hellman (ECDH) shared secret logic.  
  * Create the submitLikes function to generate SHA-256 hashes of the shared secret and push them to the database.  
  * Implement logic to encrypt plaintext choices and upload them to the encrypted_vault.  
  * Ensure local RAM is securely wiped of choices post-submission.
  * Implement the logic to match users choices to the downloaded json file.
  * Implement logic to decrypt local storage using the pin.

---

## Design Resources

Will be updated soon.

---

## Getting Help

If you have questions or need assistance:

* Open an issue on the GitHub repository.
* Reach out out the maintainers in the discord channel.

*NOTE:* Refrain from using DMs for questions. Do not use emojis or foul language in commit messages.
