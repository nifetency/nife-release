# Nife CLI

**Nife CLI** is a command line interface to the launchnife.io platform that allows users to manage authentication, application initialization, deployment, network configuration, logging, and more with just one command.

## Installation

You can install the Nife CLI using the installers below, or download a release binary from the [https://github.com/nifetency/nife-release/releases/tag/prod-v0.3.5](https://github.com/nifetency/nife-release/releases/tag/prod-v0.3.5)

### macOS and Linux

1. Launch the terminal.
2. Run the following command:
    ```sh
    curl -L https://api.nife.io/release/install.sh | sh
    ```
    This command creates a `.nife` folder and adds Nife CLI to the PATH variable.

### Windows

1. Launch the command prompt.
2. Run the following command:
    ```powershell
    iwr https://api.nife.io/release/install.ps1 -useb | iex
    ```

### Homebrew (macOS and Linux)

If you use Homebrew, you can install the Nife CLI with the following commands:

1. Set up the brew tap:
    ```sh
    brew tap nifetency/homebrew-tap
    ```
2. Install the CLI directly from brew:
    ```sh
    brew install nifetency/tap/nifectl
    ```
    You can manage all upgrades to the CLI from the Homebrew Tap.

## Usage

After installation, you can use the Nife CLI to manage your Nife.io applications. Here are some common commands:

- **Initialize an App**:
    ```sh
    nifectl init
    ```
- **Deploy an App**:
    ```sh
    nifectl deploy
    ```
- **Open a Deployed Web Application**:
    ```sh
    nifectl open
    ````

### Full Command List

For a full list of available commands, you can use the help command:
```sh
nifectl help

Available Commands:

    apps: Manage Apps
    auth: Manage authentication
    builtins: View and manage Nifectl deployment builtins
    cluster: Bring your own cluster (BYOC)
    config: Manage an App's configuration
    dashboard: Open web browser on Nife Web UI for this app
    deploy: Deploy an App to the Nife platform
    destroy: Permanently destroys an App
    docs: View Nife documentation
    help: Help about any command
    history: List an App's change history
    init: Initialize a new application
    list: Lists your Nife resources
    logs: View App logs
    metrics: List App metrics
    move: Move an App to another organization
    open: Open browser to current deployed application
    orgs: Commands for managing Nife organizations
    platform: Nife platform information
    regions: Manage regions
    releases: List App releases
    resume: Resume an application
    secrets: Manage App secrets
    status: Show App status
    suspend: Suspend an application
    version: Show version information for the Nife CLI
    workload: Commands for managing Nife workload management

Documentation

For detailed documentation, visit the [Nife Documentation](https://docs.nife.io/docs/CLI/help).

If you encounter any issues or have questions, please open an issue on the GitHub issues page or contact our support team at hello@nife.io.
