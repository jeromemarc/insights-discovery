# Red Hat Discovery - Ansible Playbook for Automated Upload to Red Hat Insights Inventory

# Overview
This project provides an Ansible playbook that automates the process of uploading completed Discovery Reports into the Red Hat Inventory. With this playbook, system administrators and DevOps teams can easily automate and schedule the upload process, saving time and reducing manual errors.

# Prerequisites
* Red Hat Discovery server is available and configured.
* Red Hat Discovery server provides successfully completed reports ready for upload.
* Red Hat Insights is avaiable for the organization.

# Demonstration

[dsc_insights_upload_playbook.webm](https://github.com/user-attachments/assets/a782607d-9c2e-40ad-b519-548811571156)

# Getting Started

## 1. Clone the Repository
First, clone the repository to your local machine:

```
git clone https://github.com/jeromemarc/insights-discovery.git
cd insights-discovery
```

## 2. Configure the Playbook
You need to configure a few variables before running the playbook:

```
dsc_server: IP address for the Discovery server
dsc_port: Port for the Discovery server (default is 9443)
dsc_username: Username for the Discovery Server
dsc_password: Password for the Discovery Server
```

## 3. Run the Playbook
Once you’ve configured the playbook, run it using the following command:

```
ansible-playbook dsc_upload.yml
```

This will execute the playbook, and your Discovery Reports will be uploaded to the Red Hat Insights Inventory.

## 4. Verify the Upload
Check the Red Hat Insights inventory or use its API to verify that the Discovery Report has been successfully uploaded.

# Additional Resources
* [Installing and Configuring Discovery](https://docs.redhat.com/en/documentation/subscription_central/1-latest/html/installing_and_configuring_discovery/index)
* [Using Discovery](https://docs.redhat.com/en/documentation/subscription_central/1-latest/html/using_discovery/index)
* [Troubleshooting Discovery](https://docs.redhat.com/en/documentation/subscription_central/1-latest/html/troubleshooting_discovery/index)
* [Viewing and managing system inventory in Insights](https://docs.redhat.com/en/documentation/red_hat_insights/1-latest/html/viewing_and_managing_system_inventory/index)
 
# Contributing
Contributions to this project are welcome! If you have suggestions, improvements, or bug fixes, feel free to open an issue or submit a pull request.

