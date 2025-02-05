# Ansible Project

## Overview
This project utilizes Ansible to automate IT infrastructure and application deployment. It includes basic and advanced system setup playbooks written entirely in Jinja.

## Repository Structure

   ```
.
└── ansible
├── README.md
├── advance_function.yml
├── inventory.ini
├── system_setup.yml
└── templates
└── zshrc.j2
   ```

## Features
- Automates configuration management
- Supports various modules for different tasks
- Written in Jinja for templating

## Playbooks
### Basic System Setup (`system_setup.yml`)
- Updates and upgrades Homebrew packages
- Creates a new user
- Installs common packages with Homebrew
- Sets timezone
- Ensures SSH service is running

### Advanced System Setup (`advance_function.yml`)
- Updates and upgrades Homebrew packages
- Adds required Homebrew taps
- Installs development tools and Docker Desktop
- Installs and configures Oh My Zsh
- Configures Git
- Installs VS Code extensions
- Configures macOS preferences
- Creates common directories

## Requirements
- Ansible installed on your local machine
- Python installed on your local machine

## Installation
1. Clone the repository:
    ```bash
    git clone https://github.com/dennislee928/ansible.git
    ```
2. Navigate to the project directory:
    ```bash
    cd ansible
    ```

## Usage
1. Update the `inventory.ini` file with your server details.
2. Run the playbooks using the following commands:
    ```bash
    ansible-playbook system_setup.yml
    ansible-playbook advance_function.yml
    ```

## Contribution
Feel free to contribute by opening issues or submitting pull requests.

## License
This project is licensed under the MIT License. See the `LICENSE` file for more details.
