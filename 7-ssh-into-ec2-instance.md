ssh into EC2 instance


1. check port 22 - TCP is open in the inbound rules in Security group of EC2


2. ssh using .pem file ```ssh -i ec2-ssh.pem ec2-user@public-ip-of-ec2-instance```  
   1. ec2-user --> is the linux user of the EC2 machine
   

3. chmod 400 .pem file. ``` 400 protects it by making it read only and only for the owner.```

--------------

EC2 instance Connect -> browser based (behind the scenes - its ssh) 

    -> still needs the Security Group open for port 22 
    -> comes with aws-cli
    -> will need to do aws configure 
        -> BAD idea -> bcoz if u put your personal creds there
            -> then anyone else in our account can connect to our EC2 instance using EC2 connect
                -> & retrive our access id & secret key

    -> instead we should use IAM role
        -> attach an IAM role to the EC2 instance 
        -> then u dont need to do aws configure
    
    

