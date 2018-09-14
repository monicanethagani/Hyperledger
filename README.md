# Hyperledger
All the pre-requisites required are installed and the versions are verified and are shown below:
 
1.	The following commands were used:
•	Curl- sudo apt install curl
•	Pyhton- It was already in the required version
•	Node- sudo apt-get install nodejs
           sudo apt-get install npm
•	Go- sudo apt-get update
sudo apt-get -y upgrade
wget https://d1.google.com/go/go1.10.3.linux-amd64.tar.gz
sudo tar -xvf go1.10.3.linux-amd64.tar.gz
sudo mv go /usr/local
here the set path is supposed to be set.
•	Docker- curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add –
•	Docker Compose-  sudo curl -L ”https://github.com/docker/compose/releases/download/1.22.0/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
•	After the docker is installed successfully, the system was shut down and then started again for the changes to be made.

2.	Now, enter into the first network directory which was created and give the command: ./byfn.sh -m generate
3.	This command generates the certificates required for the first network and to see what have been generated give the following command: 
cd crypto-config
ls
If the genesis block and all the channels are generated, then it means that the it is created successfully.
4.	To create the first network, the following command is used:
$ ./byfn.sh -m up
If all the drivers have been installed and the START  and END appears, it means that the first network is built successfully.
5.	The peers generated are shown in the following image. To bring down the created network executed the following command:
$ ./byfn.sh -m down
6.	Then the images which were generated have been discarded. 
