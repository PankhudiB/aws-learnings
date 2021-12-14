#IAM

IAM 
    
    identity & Access Management
    - Global Service
    - root a/c -> dont use/share
    - Users - ppl in org
        - can be grouped
            - devs / ops / audit
        - groups cant contain other groups 
        - user can belong to multiple groups
        - u can add **TAGS** to user    
Why create users/groups ?
    
    For Permissions
        -> JSON doc -> Policy
    -> Follow the least privilage principle

u can create alias to your account

Policy 

has :

- version --> date
- Id --> optional
- array of statements :
  - id of statement
  - Effect -> to allow/deny access to certain API
  - Principal -> account/user/role it applies to
  - Actions -> list of APIs that r being allowed/denied access based on Effect
  - Resource -> list of resources actions applies to
  - Condition -> when this policy is in effect (optional)
  

        
        
