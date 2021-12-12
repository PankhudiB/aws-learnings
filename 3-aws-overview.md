##AWS overview

AWS Regions 
        
    cluster of datacenters
    most aws services - region scoped

How to choose AWS region ?

    factors :
    1. complaince -> sometimes govt wants it to be in their own region
    2. proximity to customers -> reduced latency
    3. not all regions have all AWS services
    4. pricing -> varies from region to region
    
AWS Availibility Zones
    
    each Region has many AZ 
    Each AZ -> is 1/more descrete datacenters with redundant power,n/w, connectivity
    -> separate -> in order to isolate from disasters
    these AZs are connecteded with high bandwidth & ultra-low latency n/w

AWS Points of Presence
    
    like edge locations 