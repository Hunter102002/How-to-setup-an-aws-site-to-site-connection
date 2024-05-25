# Setting up an AWS Site-to-Site (S2S) VPN Connection

## Objective

This project aimed to establish a Site-to-Site VPN connection between an on-premises network and an AWS VPC to enable secure communication between resources in both networks. The project demonstrates advanced-level skills in configuring AWS VPC, EC2 instances, Customer Gateway, Virtual Private Gateway, and setting up IPsec VPN connections.

### Skills Learned

- AWS VPC Management: Creating and managing VPCs, subnets, route tables, and internet gateways.
- VPN Configuration: Establishing a Site-to-Site VPN connection using AWS VPN and configuring IPsec tunnels.
- EC2 Management: Launching and configuring EC2 instances to act as routers and test connectivity.
- Network Security: Setting up security groups and firewall rules for secure communication.
- Advanced Networking: Configuring Customer Gateway and Virtual Private Gateway for VPN connections.

### Tools Used

- Amazon EC2: For launching and managing virtual machines.
- Amazon VPC: For creating and managing VPCs and related networking components.
- AWS VPN: For setting up and managing Site-to-Site VPN connections.
- AWS Management Console: For configuring and managing all AWS resources.


### Outcome
The project successfully demonstrated the setup of a Site-to-Site VPN connection, allowing secure communication between an on-premises network and an AWS VPC. By completing this project, I have showcased advanced networking skills and the ability to configure secure communication channels between different networks using AWS services.

## Steps

Create a VPC in Mumbai Region

![Screenshot 2024-05-22 at 4 40 44 PM](https://github.com/Hunter102002/How-to-setup-an-aws-site-to-site-connection/assets/98543129/2d7f0798-2e4c-4493-95e8-46b306500d6f)

Create a public subnet

![Screenshot 2024-05-22 at 4 42 17 PM](https://github.com/Hunter102002/How-to-setup-an-aws-site-to-site-connection/assets/98543129/9d63ce97-079d-40d8-9632-a8d30f85874d)

Create and attatch Internet Gateway

![Screenshot 2024-05-22 at 4 43 07 PM](https://github.com/Hunter102002/How-to-setup-an-aws-site-to-site-connection/assets/98543129/66dbb478-f3c1-49d7-b00f-21e0a18c05f4)

![Screenshot 2024-05-22 at 4 43 18 PM](https://github.com/Hunter102002/How-to-setup-an-aws-site-to-site-connection/assets/98543129/801c3dcf-4c72-41b1-8619-94d44c8358ac)

Create public route table and associate with the subnet

![Screenshot 2024-05-22 at 4 45 12 PM](https://github.com/Hunter102002/How-to-setup-an-aws-site-to-site-connection/assets/98543129/d2ea2702-3767-4582-97d2-f608c7a2e396)

Add a Public route 

![Screenshot 2024-05-22 at 4 46 10 PM](https://github.com/Hunter102002/How-to-setup-an-aws-site-to-site-connection/assets/98543129/24338a3e-de4e-4ce8-9ac9-78825fe4e66f)

Create an EC2 instance

![Screenshot 2024-05-22 at 4 51 00 PM](https://github.com/Hunter102002/How-to-setup-an-aws-site-to-site-connection/assets/98543129/15042ef4-e988-41a1-86d1-48012012134a)

Create a VPC in US-East1 Region

![Screenshot 2024-05-22 at 4 52 01 PM](https://github.com/Hunter102002/How-to-setup-an-aws-site-to-site-connection/assets/98543129/70252258-3dfe-4dbc-b74c-64d89c11a6a3)

Create and attach Private subnet

![Screenshot 2024-05-22 at 4 53 08 PM](https://github.com/Hunter102002/How-to-setup-an-aws-site-to-site-connection/assets/98543129/5e5d7c82-b499-4266-aa84-58fe24f6224b)

Launch EC2 instance

![Screenshot 2024-05-22 at 4 56 27 PM](https://github.com/Hunter102002/How-to-setup-an-aws-site-to-site-connection/assets/98543129/dbe7e537-8723-45ca-b419-0e095e9a1d13)

Create a cusotmer gateway in US-East1 Region

![Screenshot 2024-05-22 at 4 58 39 PM](https://github.com/Hunter102002/How-to-setup-an-aws-site-to-site-connection/assets/98543129/7637dc9c-d32d-423d-9961-50ceaebb047e)

Create a virtual private gateway 

![Screenshot 2024-05-22 at 4 59 32 PM](https://github.com/Hunter102002/How-to-setup-an-aws-site-to-site-connection/assets/98543129/48bb8511-e8de-4d9d-af18-084ae5bf8843)

Create the VPN Connection 

![Screenshot 2024-05-22 at 5 07 14 PM](https://github.com/Hunter102002/How-to-setup-an-aws-site-to-site-connection/assets/98543129/08156b6e-3bb7-4466-816e-fe19e6706657)

Launch instance and ssh into onstance to verify connection

![Screenshot 2024-05-22 at 5 09 13 PM](https://github.com/Hunter102002/How-to-setup-an-aws-site-to-site-connection/assets/98543129/684f3761-bf10-495a-9465-8d7efd9bdc6c)


![Screenshot 2024-05-22 at 5 13 23 PM](https://github.com/Hunter102002/How-to-setup-an-aws-site-to-site-connection/assets/98543129/cd85175a-701e-439a-a7fb-5007cc47e828)
