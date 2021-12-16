##Security Group

    its like a firewall on EC2 instance 
    controls traffic in & out of EC2 instance 
    SG -> rules by IP address/ranges or other SG
    they also regulate access to ports
    

    EC2 instance 1                  EC2 instance 2
        SG - 1           <--            SG-1
        SG - 2                                  
                          <-------   EC2 instance 3  
                                         SG-2
------------------

    1 SG -> can be applied to multiple instance
    1 instance can have multiple SG
    Good to maintain separate SG for SSH access
------------------

    If ur app is giving time out --> SG issue
    IF it gave "connection refused" error 
        --> then SG actually worked -> and request went through
------------------

    Classic ports to know

    PORT    
    22 --> allows SSH (secure shell) -> log in to Linux instance
    21 --> FTP  --> upload file
    22 -> Secure FTP --> upload file using ssh
    80 --> http (non secure)
    443 --> https
    3389 --> RDP remote desktop protocol -> logging into window desktop
------------------



    
