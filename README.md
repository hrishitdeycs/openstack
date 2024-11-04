# openstack
### 1.Create an account on aws
### 2.Sign in to your account 
### 3.Go to your dashboard
### 4.Click on launch instance
### 5.Enter your server name and select ubuntu(22.04)
### 6.Click on create new key pair
### 7.Enter your key pair name then select .ppk and click on create new key pair
### 8.In the network settings click on allow all traffic from the internet
### 9.Increase storage to 50gb then Click on launch instance
### 10.Copy the public ipv4 address from your instance and download putty. 
### 11.Paste the ip address in host name   
### 12.Click on SSH then auth then credentials
### 13.Click browse and open the key pair you downloaded
### 14.Click accept then type ubuntu and then press enter 
### 15.Use the following command to install openstack
```bash
sudo snap install openstack --channel 2024.1/beta
```
### 16.Use the following commands to create and launch vm on openstack
```bash
sunbeam prepare-node-script
```
```bash
sunbeam prepare-node-script | bash -x && newgrp snap_daemon
```
### 17.This will take around 30 mins
```bash
sunbeam cluster bootstrap --accept-defaults
```
```bash
sunbeam configure --accept-defaults --openrc demo-openrc
```
```bash
sunbeam launch ubuntu --name test
```
![Screenshot (4)](https://github.com/user-attachments/assets/4a24ee2e-d5e8-4d18-9b21-00af6155d545)

### 18.On the instance dashboard click on terminate running instance  
