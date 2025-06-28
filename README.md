![azuretf](https://github.com/user-attachments/assets/612a06b6-a6ee-414d-8829-b59564db93bd)
![azuretopo](https://github.com/user-attachments/assets/04724321-0673-46f2-9eae-99764a31ff4d)
Once the resources been created need to ssh 
Follow  the below step 
Grab the PUblic of vm 
terraform output public_ip

get the private key and save it
terraform output -raw private_key > id_rsa

Set Permissions for id rsa file 
chmod 400 id_rsa

SSH into vm 
ssh -i id_rsa azureuser@<your-public-ip>
