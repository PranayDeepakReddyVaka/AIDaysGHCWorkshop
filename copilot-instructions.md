## Operator Interaction
- When asked to fix code, first explain the problems found.
- When asked to generate tests, first explain what tests will be created.
- When making multiple changes, provide a step-by-step overview first.

## Security
- Check the code for vulnerabilities after generating.
- Avoid hardcoding sensitive information like credentials or API keys.
- Use secure coding practices and validate all inputs.

## Environment Variables
- If a .env file exists, use it for local environment variables
- If a .env file does not exist, create one with the necessary variables using the requirements.txt file
- Update the requirements.txt file whenever new dependencies are added
- Document any new environment variables in README.md

## For Python Projects Only
- Always use a Python virtual environment: if no venv exists, create one and activate
- Always use and update a requirements.txt file for Python modules
- Follow PEP 8 style guidelines
- Include type hints (PEP 484)


## Version Control
- Keep commits atomic and focused on single changes
- Follow conventional commit message format
- Update .gitignore for new build artifacts or dependencies
- If .gitignore is not present, create one with the necessary entries

## Code Style
- Follow existing project code style and conventions
- Add type hints and docstrings for all new functions
- Include comments to explain logic

## Change Logging
- Each time you generate code, note the changes in changelog.md
- If no changelog.md exists, create one with the necessary sections
- Use the format: `## [version] - YYYY-MM-DD`
- Include a section for "Added", "Changed", "Deprecated", "Removed", "Fixed", and "Security"
- Follow semantic versioning guidelines
- Include date and description of changes




