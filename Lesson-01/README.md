Install Terraform
Follow the installation guide: https://developer.hashicorp.com/terraform/install

or

Common Installation Commands

# For Windows
````text
winget install Hashicorp.Terraform
````
# For macOS
````text
brew install hashicorp/tap/terraform
````
# For Ubuntu/Debian
````text
wget -O- https://apt.releases.hashicorp.com/gpg | sudo gpg --dearmor -o /usr/share/keyrings/hashicorp-archive-keyring.gpg
echo "deb [signed-by=/usr/share/keyrings/hashicorp-archive-keyring.gpg] https://apt.releases.hashicorp.com $(lsb_release -cs) main" | sudo tee /etc/apt/sources.list.d/hashicorp.list
sudo apt update && sudo apt install terraform
````

## Setup Commands
````text
terraform -install-autocomplete
alias tf=terraform
terraform -version
````
Common Installation Error (macOS)
If you encounter:

Error: No developer tools installed.
Install Command Line Tools:

xcode-select --install

For these lessons, you will also need the AWS CLI. If you do not already have it installed, you can follow the directions below.

## AWS CLI Installation
Check your system architecture first:
````text
# Linux/macOS
uname -m

# Windows PowerShell
$env:PROCESSOR_ARCHITECTURE
Official Website: https://aws.amazon.com/cli/
````
## Windows:
````text
# Using MSI installer (recommended)
# Download from: https://awscli.amazonaws.com/AWSCLIV2.msi

# Using winget
winget install Amazon.AWSCLI
# Using chocolatey
choco install awscli
````

## macOS:
````text
# Using official installer
curl "https://awscli.amazonaws.com/AWSCLIV2.pkg" -o "AWSCLIV2.pkg"
sudo installer -pkg AWSCLIV2.pkg -target /

# Using Homebrew
brew install awscli
````

## Ubuntu/Debian:
````text
# Update package index
sudo apt update

# Install AWS CLI v2 (choose based on your architecture)
# For x86_64
curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"

# For ARM64
curl "https://awscli.amazonaws.com/awscli-exe-linux-aarch64.zip" -o "awscliv2.zip"

unzip awscliv2.zip
sudo ./aws/install

# Verify installation
aws --version
````
