# Universal System Updater and Packager Installer in Most Linux Distribution

This Git repository contains two universal system maintenance scripts that can be used on various Linux distributions. These scripts are designed to work with different package managers and are intended for system administrators or users who need to update and install packages.

## Prerequisites

Make sure you have the following prerequisites installed on your system:

- Bash (a Unix shell)
- Appropriate permissions to run system updates and install packages using `sudo`

## Scripts

### 1. Universal Update Script

**Script Name**: `update`

This script updates and upgrades your system using the appropriate package manager based on the detected distribution. It supports the following package managers:

- APT (Advanced Package Tool)
- YUM (Yellowdog Updater, Modified)
- DNF (Dandified YUM)
- Zypper
- Pacman
- Portage
- Nix

To run the script:

```bash
update
```

### 2 - Universal Package Installation Script

**Script Name**: `package`

This script allows you to install packages using the appropriate package manager based on the detected distribution. It supports the same package managers as the update script.

To install a package, run the script and provide the name of the package when prompted.

To run the script:

```bash
package *** #The name of your package
```

## Usage

1. Clone this repository to your local machine:

   ```bash
   git clone https://github.com/RedeemedSpoon/Universal-Update-Packager-Installer.git
   ```

2. Change to the repository directory:

   ```bash
   cd Universal-Update-Packager-Installer
   ```

3. Make sure the scripts have execute permissions:

   ```bash
   chmod 755 *
   ```

4. Move the scripts to /usr/bin using the sudo command, which requires administrative privileges:

   ```bash
   sudo mv * /usr/bin/
   ```
5. Run the desired script as described above.

## Contributing

If you have improvements or additional package manager support to contribute, please open a pull request with your changes.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
