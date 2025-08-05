How to Contribute to the AI HF Propagation Analyzer
First off, thank you for considering contributing to this project! Every contribution, whether it's a bug report, a feature suggestion, or a code change, is immensely valued and welcomed.

This document is a guide to make the contribution process easy and effective for everyone.

Code of Conduct
This project and everyone participating in it are governed by our Code of Conduct. By participating, you are expected to uphold this code. Please take a moment to read it to ensure a respectful environment for all.

How Can You Contribute?
There are many ways to contribute, and not all of them involve writing code.

Reporting Bugs: If you find unexpected behavior or an error, please open an Issue. Provide as much detail as possible, including steps to reproduce the problem.

Suggesting Enhancements: Have an idea for a new feature or an improvement to an existing one? Open an Issue with a clear description of your suggestion.

Writing Code: If you want to fix a bug or implement a new feature, feel free to submit a Pull Request.

Your First Pull Request
If you're ready to contribute code, follow the steps below to set up your development environment.

1. Setting Up Your Environment
Fork the repository by clicking the "Fork" button in the top-right corner of this page.

Clone your fork to your local machine. (Remember to replace YOUR_USERNAME and YOUR_REPOSITORY):

git clone https://github.com/YOUR_USERNAME/YOUR_REPOSITORY.git

Navigate to the project directory:

cd YOUR_REPOSITORY

Install the project dependencies. This project uses npm.

npm install

Set Up Environment Variables: The project requires an API key to communicate with the Anthropic service.

Create a file named .env.local in the root of the project.

Inside this file, add your API key. The .gitignore file is already configured to ignore this file, ensuring your key is not sent to GitHub.

ANTHROPIC_API_KEY=your_api_key_here

Note: A future implementation will move the use of this key to the backend for security.

Run the Development Server:

npm run dev

You can now access the project at http://localhost:3000 and start making your changes!

2. Pull Request (PR) Process
Create a New Branch: From the main branch of your fork, create a descriptive branch for your change.

git checkout -b feat/add-new-chart
# or
git checkout -b fix/correct-input-bug

Make Your Changes: Write your code, always keeping the existing style and patterns of the project in mind.

Check Code Quality: Before committing, run the linter to ensure your code follows the project's standards.

npm run lint

Commit Your Changes: Use clear and descriptive commit messages. We recommend the Conventional Commits standard.

git commit -m "feat: Add comparison chart for day and night bands"

Push Your Branch to Your Fork:

git push origin feat/add-new-chart

Open a Pull Request: Go to the original repository's page on GitHub, and you will see a prompt to open a Pull Request from your new branch. Fill out the PR template with a clear description of what you did and why.

Style Guides
Commit Messages
We use the "Conventional Commits" standard. This helps us maintain a clean commit history and automate the generation of changelogs. The format is:

<type>[optional scope]: <description>

Common types: feat (new feature), fix (bug fix), docs (documentation), style (formatting), refactor (code refactoring), test (adding tests).

Code Style
The project uses TypeScript for more robust code.

Styling is done with Tailwind CSS.

Please follow the standards defined by ESLint, which can be checked with the npm run lint command.

License
By contributing, you agree that your contributions will be licensed under the project's MIT License.