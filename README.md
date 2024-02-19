# Create a VM in Azure to Deploy a Web Server

In this project, we are going to focus on eight points:

- Create a Resource Group

- Create a Virtual Network and a subnet

- Protect a subnet using a Network Security Group

- Deploy Bastion to connect to a Virtual Machine

- Create an Ubuntu Server Virtual Machine

- Install Nextcloud by connecting via SSH using Bastion

- Publish an IP

- Create a DNS label

In this project we will learn the basic networking architecture in Azure works, by creating Virtual Networks, subnets, security groups and Virtual Machines. We will also learn how to use Bastion to connect to a Linux machine using SSH without exposing and external IP. We will learn how to expose a public IP and an HTTPS port to access your web server.

# Architecture

![Screenshot 2024-02-19 at 00 04 35](https://github.com/redjules/Create-a-VM-in-Azure-to-Deploy-a-Web-Server/assets/106017493/88ba6f84-7ce9-46bd-b343-376e66d47d75)

First we create a resource group in Azure:

![Screenshot 2024-02-19 at 00 11 38](https://github.com/redjules/Create-a-VM-in-Azure-to-Deploy-a-Web-Server/assets/106017493/e19d8591-a0c2-4806-ba9e-7b3ee69b5ff3)

![Screenshot 2024-02-19 at 00 13 01](https://github.com/redjules/Create-a-VM-in-Azure-to-Deploy-a-Web-Server/assets/106017493/6b038bff-0662-4729-9774-9047b27d32a5)

Then we create a virtual network and a subnet in Azure:

![Screenshot 2024-02-19 at 00 18 58](https://github.com/redjules/Create-a-VM-in-Azure-to-Deploy-a-Web-Server/assets/106017493/4b69a65b-aa39-4032-888c-f22c767b3c29)

![Screenshot 2024-02-19 at 00 29 43](https://github.com/redjules/Create-a-VM-in-Azure-to-Deploy-a-Web-Server/assets/106017493/15a2f632-0a74-429c-96c9-0a4dce16fb58)

![Screenshot 2024-02-19 at 00 30 36](https://github.com/redjules/Create-a-VM-in-Azure-to-Deploy-a-Web-Server/assets/106017493/2a53ca94-c534-4204-852f-007798a03d32)


we add a network security group to our resource:

![Screenshot 2024-02-19 at 00 56 17](https://github.com/redjules/Create-a-VM-in-Azure-to-Deploy-a-Web-Server/assets/106017493/b02e29b0-272a-4ad5-a2f2-ead2738eceba)

![Screenshot 2024-02-19 at 00 58 00](https://github.com/redjules/Create-a-VM-in-Azure-to-Deploy-a-Web-Server/assets/106017493/e2d78c5d-c194-4ec9-ba8d-b8c962718afb)

![Screenshot 2024-02-19 at 00 58 40](https://github.com/redjules/Create-a-VM-in-Azure-to-Deploy-a-Web-Server/assets/106017493/85df72f2-1f7f-4def-b6d8-27797b8da775)

we create a new subnet (AzureBastionSubnet):

![Screenshot 2024-02-19 at 01 12 52](https://github.com/redjules/Create-a-VM-in-Azure-to-Deploy-a-Web-Server/assets/106017493/8850936a-78af-4242-a048-57207552cc94)


![Screenshot 2024-02-19 at 01 15 05](https://github.com/redjules/Create-a-VM-in-Azure-to-Deploy-a-Web-Server/assets/106017493/be9fa3e7-fe09-4af1-b4a2-850bba0b3ed7)

now we create a virtual machine:

![Screenshot 2024-02-19 at 01 27 01](https://github.com/redjules/Create-a-VM-in-Azure-to-Deploy-a-Web-Server/assets/106017493/6f60cb15-6cb9-45fc-bb82-c16a06527685)

and connect with Bastion:

![Screenshot 2024-02-19 at 02 36 03](https://github.com/redjules/Create-a-VM-in-Azure-to-Deploy-a-Web-Server/assets/106017493/a4bacf3c-ec1b-412e-85a9-fab2729e7079)

