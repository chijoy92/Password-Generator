# Keyforge | Password Generator

A modern, secure, and responsive Password Generator built with **HTML, CSS, and JavaScript**.

Keyforge allows users to generate strong random passwords and memorable passphrases with customizable settings, password strength feedback, and one-click copying.

The application works entirely in your browser without requiring a backend, database, registration, or API key.

## Features

- Generate secure random passwords between 8 and 64 characters
- Customize password length
- Include or exclude uppercase letters, lowercase letters, numbers, and symbols
- Automatically include at least one character from every selected category
- Exclude easily confused characters such as `0`, `O`, `1`, `l`, and `I`
- Generate memorable passphrases containing 3 to 8 words
- Customize passphrase capitalization and number suffixes
- Copy generated passwords with one click
- View approximate password strength
- Modern and responsive user interface
- Secure password generation using the Web Crypto API
- No backend, database, or API keys required

## Technologies Used

| Technology | Purpose |
|---|---|
| HTML5 | Application structure |
| CSS3 | Styling and responsive design |
| JavaScript | Password generation and interaction |
| Web Crypto API | Cryptographically secure random values |
| Node.js | Optional automated testing |

## Installation and Setup in VS Code

### Step 1: Download the Project

1. Click the green **Code** button on this GitHub repository.
2. Select **Download ZIP**.
3. Extract the downloaded ZIP file.
4. Open Visual Studio Code.
5. Select **File > Open Folder**.
6. Choose the extracted `password-generator` folder.

### Step 2: Run the Application

No installation is required.

1. Open the project folder.
2. Locate the `index.html` file.
3. Double-click `index.html` to open it in your browser.
4. The Password Generator is ready to use.

The application works without installing Python, Node.js, or a backend server.

### Alternative: Run Using Live Server

You can also run the project using the Live Server extension in VS Code.

1. Open VS Code.
2. Go to the Extensions panel.
3. Search for **Live Server** by Ritwick Dey.
4. Install the extension.
5. Open `index.html`.
6. Right-click and select **Open with Live Server**.

The website will typically open at:

`http://127.0.0.1:5500`

## How to Use

### Generate a Random Password

1. Open the Password Generator.
2. Select **Random password**.
3. Choose your preferred password length.
4. Enable or disable uppercase letters, lowercase letters, numbers, and symbols.
5. Enable the option to exclude confusing characters if needed.
6. Click **Generate new secret**.
7. Click **Copy** to copy your password to the clipboard.

### Generate a Memorable Passphrase

1. Select **Memorable passphrase**.
2. Choose the number of words.
3. Customize capitalization and number suffix settings.
4. Click **Generate new secret**.
5. Copy the generated passphrase.

## Project Structure

```text
password-generator/
├── index.html
├── assets/
│   ├── app.js
│   ├── core.mjs
│   └── styles.css
├── tests/
│   └── core.test.mjs
├── .gitignore
├── LICENSE
└── README.md
```

### File Descriptions

- **index.html:** Contains the main application interface.
- **assets/styles.css:** Handles the styling, layout, and responsive design.
- **assets/app.js:** Manages user interactions, password generation, and clipboard functionality.
- **assets/core.mjs:** Contains independently testable password generation logic.
- **tests/core.test.mjs:** Contains automated tests.
- **.gitignore:** Excludes unnecessary development files.
- **LICENSE:** Contains the MIT License.

## Running Automated Tests

Node.js version 18 or newer is required only for running automated tests.

Open the VS Code terminal:

**Terminal > New Terminal**

Execute:

```bash
node --test tests/core.test.mjs
```

The automated tests cover:

- Password length validation
- Character category selection
- Secure random number handling
- Character exclusion rules
- Passphrase generation
- Password configuration validation

**Note:** Node.js is not required to run the actual website.

## Deploying on GitHub Pages

This project can be hosted for free using GitHub Pages.

### Deployment Steps

1. Create a public GitHub repository named `password-generator`.
2. Upload all project files and folders.
3. Ensure `index.html` is in the repository's root directory.
4. Open your repository's **Settings**.
5. Click **Pages**.
6. Under **Build and deployment**, choose **Deploy from a branch**.
7. Select the `main` branch.
8. Select the `/(root)` folder.
9. Click **Save**.

Once deployment is complete, GitHub Pages will provide a public URL for your website.

## Security and Privacy

- Password generation happens locally in your browser.
- The application uses the Web Crypto API for secure random number generation.
- Generated passwords are not sent to an external server.
- Passwords are not saved in Local Storage.
- No registration or personal information is required.
- The password strength meter provides an approximate estimate, not a comprehensive security audit.
- The passphrase generator uses a limited bundled word list, so long random passwords are recommended for sensitive accounts.
- Clipboard contents may be accessible to other applications.

For better account security, use unique passwords and enable two-factor authentication whenever possible.

## Browser Compatibility

The application is designed for modern browsers, including:

- Google Chrome
- Microsoft Edge
- Mozilla Firefox
- Safari

## Contributing

Contributions, suggestions, and improvements are welcome.

1. Fork this repository.
2. Create a new branch.
3. Make your changes.
4. Test your changes.
5. Submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE).

You are free to use, modify, and distribute the source code according to the license terms.
