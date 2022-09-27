# NGINX_AWS
Setup NGINX web server using AWS EC2 instance

## AWS SETUP
Launch a EC2 instance with the below requirements. 
1. Amazon Machine Image - Ubuntu Server of 64-bit (x86) machine (Free-tier)
2. Instance type - t2-micro (Free-tier)
3. Key-pair - Create a new key-pair or use an already-existing one.
4. Security groups - Allow all SSH, HTTP and HTTPS traffics. ( You can customize the incoiming and outgoing traffic as required )
	
	<img width="536" alt="image" src="https://user-images.githubusercontent.com/48701982/192517785-c23f2cd4-3c60-4318-9c1f-3ad564b629b7.png">

	
5. Launch the instance with all the other settings left unchanged.

## Install NGINX
1. With EC2 instance connect, connect the launched instance.

	<img width="284" alt="image" src="https://user-images.githubusercontent.com/48701982/192517282-55425332-47ef-45ce-9d50-e06eb81b65ee.png">

2. To install nginx, adhere to the steps provided.
		
		sudo apt-get update
		sudo apt-get install nginx
		nginx -v
		sudo systemctl status nginx
		
3. Navigate to AWS EC2 console and you can see the instance’s public IP address in the Public IPv4 address column of your launched instance. 
4. Copy the public IP address and paste it in the browser. (Eg : http://<public_IP_addr>/)
5. The default Welcome to nginx! page appears, indicating that NGINX is installed and running but not yet configured.
         
	 <img width="463" alt="image" src="https://user-images.githubusercontent.com/48701982/192517939-a4f21670-82e4-4953-ae75-ee24ebaafde1.png">

