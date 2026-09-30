


# Copilot Workflows

All project documents are now fully functional.

Currently available workflow tasks:

- Generate

Currently available Bones Generator Targets:

- README.md
- CHANGELOG.md
- CONTRIBUTING.md
- LICENSE
- API documentation
- Architecture diagrams
- Deployment diagrams
- User guides
- Developer guides

This project demonstrates how to use Copilot-driven workflows to automate project documentation and file generation. The workflow system can generate and maintain all standard documentation files, API docs, diagrams, and guides for your project. All generated documents are now fully functional and ready for use.

## Introduction

Copilot Workflows is a system for automating common project tasks, such as generating documentation, using a workflow-driven approach. It leverages PowerShell scripts and Copilot instructions to streamline project setup and maintenance.

## Installation

1. Clone this repository to your local machine.
2. Ensure you have PowerShell (pwsh) installed.
3. Review and customize the workflow scripts and skeleton templates in the `skeleton/docs` directory as needed.

## Usage

To trigger a documentation workflow, use the following chat command:

```powershell
workflows project document
```

This will generate all standard documentation files for your project, including:

- README.md
- CHANGELOG.md
- CONTRIBUTING.md
- LICENSE
- API documentation
- Architecture diagrams
- Deployment diagrams
- User guides
- Developer guides

## Command Tree

```tree
   workflows
     |
     |+-- project
     |       |
     |       |+-- document
     |       |+--
     |+--
```

## Contributing

Contributions are welcome! Please see the `CONTRIBUTING.md` file for guidelines.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

## Trademarks and non-affiliation

Product and company names in this repository belong to their owners and are used only to say what this project works with. HF Laboratories is not affiliated with, endorsed by, or sponsored by any of them.

- Microsoft and PowerShell are trademarks or registered trademarks of Microsoft Corporation.
- GitHub Copilot is a trademark or registered trademark of GitHub, Inc.

See [hflabs.dev/legal/trademarks](https://hflabs.dev/legal/trademarks) for the full list.
