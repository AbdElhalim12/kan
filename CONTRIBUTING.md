# Contributing to Kan

Thank you for your interest in contributing to Kan! This document provides guidelines and instructions for contributing to the project.

## Getting Started

1. Fork the repository
2. Clone your fork: `git clone https://github.com/YOUR-USERNAME/kan.git`
3. Create a new branch: `git checkout -b feat/your-feature-name`
4. Install dependencies: `pnpm install`
5. Copy `.env.example` to `.env` and configure your environment variables
6. Make your changes
7. Commit your changes: `git commit -m "feat: description of changes"`
8. Push to your fork: `git push origin feat/your-feature-name`
9. Open a Pull Request

you will need postgresSQL Database, head to : https://www.postgresql.org/download/ and install it. Then in pgAdmin4 create database.

- Copy .env.example file: `cp .env.example .env`
- In the .env file you will need to edit this line: `POSTGRES_URL= # e.g. postgresql://kan:your_password@your_host:5432/kan to your databse owner's username and password.`
- Run `openssl rand -base64 24 | tr -dc 'a-zA-Z0-9' | head -c 32 ` and copy that key and add it to BETTER_AUTH_SECRET=`YOUR KEY HERE`


for using e-mails without OTP or AUTH set:
`NEXT_PUBLIC_ALLOW_CREDENTIALS= true
NEXT_PUBLIC_DISABLE_SIGN_UP= false`

## Development Guidelines

### Code Style

- Follow the existing code style
- Use meaningful variable and function names
- Add comments for complex logic
- Keep functions focused and concise

### Commits

- Use clear and descriptive commit messages
- Reference issue numbers when applicable
- Keep commits focused on single changes

### Pull Requests

- Provide a clear description of the changes
- Include screenshots for UI changes
- Keep PRs focused on a single feature/fix

## Need Help?

- Join our [Discord server](https://discord.gg/e6ejRb6CmT) for questions
- Check existing issues and pull requests
- Email [henry@kan.bn](mailto:henry@kan.bn) for major concerns

## Code of Conduct

Please note that this project is released with a Contributor Code of Conduct. By participating in this project you agree to abide by its terms.

We aim to foster an inclusive and welcoming community. Harassment and abusive behavior will not be tolerated.

## License

By contributing to Kan, you agree that your contributions will be licensed under the AGPLv3 License.
