# Terraform Resources
## This project includes tools, scripts and examples for diffrent Terraform resources frequently used within Devops practices and Workflows  

### Useful information to use Terraform
Ensure that your system is up to date and you have installed the gnupg, software-properties-common, and curl packages installed. You will use these packages to verify HashiCorp's GPG signature and install HashiCorp's Debian package repository.

>$ sudo apt-get update && sudo apt-get install -y gnupg software-properties-common>

### Install the HashiCorp GPG key.

>$ wget -O- https://apt.releases.hashicorp.com/gpg | \
gpg --dearmor | \
sudo tee /usr/share/keyrings/hashicorp-archive-keyring.gpg > /dev/null

### Verify the key's fingerprint.
>$ gpg --no-default-keyring \
--keyring /usr/share/keyrings/hashicorp-archive-keyring.gpg \
--fingerprint

