# Development Environment Setup

Tools we will need:

- Terminal
- Git
- Node.js (version 20 or 22 only)
- VSCode (or your code editor of choice)

Installation instructions for each OS:

- [Mac OS](#mac-os)
- [Windows OS](#windows-os)
- [Ubuntu/WSL](#ubuntuwsl)

Recommended VSCode extensions:

- Prettier (`esbenp.prettier-vscode`)
- ESLint (`dbaeumer.vscode-eslint`)
- ES7+ React/Redux/React-Native snippets (`dsznajder.es7-react-js-snippets`)
- DotENV (`mikestead.dotenv`)
- Tailwind CSS IntelliSense (`bradlc.vscode-tailwindcss`)

> _NOTE:_ there are many similarly named extensions in VSCode and not all are high quality. To ensure you're installing the correct one search for the publisher ID provided in parentheses above.

## Mac OS

Open your **terminal.app** or [iTerm2.app](https://iterm2.com/)

> press `COMMAND+SPACE` keys, type `terminal.app`, press `return` to launch

Install the XCode Command Line tools:

```bash
xcode-select --install
```

> If you get an error saying the command line tools are already installed you can proceed with the instructions

Install [Homebrew](https://brew.sh/) with the following command:

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

**Close and Restart your terminal**

If you don't have `git` or VSCode already installed you can install with the following commands:

```bash
brew install git
brew install curl
brew tap "homebrew/cask"
brew install --cask visual-studio-code
```

Install Node.js 20

```bash
# installs nvm (Node Version Manager)
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh | bash

# download and install Node.js (you may need to restart the terminal)
nvm install 20

# verifies the right Node.js version is in the environment
node -v # should print `v20.16.0` or newer

# verifies the right npm version is in the environment
npm -v # should print `10.8.1` or newer
```

## Windows OS

Download and Install the following applications (_if you don't already have them installed_):

> The following assumes you're on a 64bit Windows computer. If you're on a 32bit computer choose those versions instead.

- **Git** (64bit) Windows setup (https://git-scm.com/download/win)
- **VS Code** (64bit) (https://code.visualstudio.com/)
- **Node.js (LTS version)** version 20 (64bit)
  - Choose the right version for your computer here: https://nodejs.org/en/download/prebuilt-installer
  - You do **NOT** need to install [Chocolatey](https://chocolatey.org/)

To run VS Code, open VS Code from your Windows/Start Menu

## Ubuntu/WSL

Install git and curl if you don't already have them installed

```bash
apt-get install git
apt-get install curl
```

Install NVM and Node.js 20

```bash
# installs nvm (Node Version Manager)
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh | bash

# download and install Node.js (you may need to restart the terminal)
nvm install 20

# verifies the right Node.js version is in the environment
node -v # should print `v20.16.0` or newer

# verifies the right npm version is in the environment
npm -v # should print `10.8.1` or newer
```

Install VSCode or use a code editor of your preference

https://code.visualstudio.com/docs/setup/linux
