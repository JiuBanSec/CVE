* VULNERABLE: SQL injection vulnerability exists in Online Pre-owned Used Car Showroom Management System. An attacker can inject query in
“/classes/Login.php" via the "username" parameters.
* Product: Online Pre-owned Used Car Showroom Management System.
* Software: https://www.sourcecodester.com/php/15067/online-pre-ownedused-car-showroom-management-system-php-free-source-code.html
* Impact: Allow attacker inject query and access , disclosure of all data on the system.
* Payload : `username=admin' and 1=1#` `username=admin' and 1=2#` `username=test' or 1=1#`
* Proof of concept (POC):

![图片](https://user-images.githubusercontent.com/57030243/160413889-fa15fe59-26b9-4abf-bec9-9b3b15027d12.png)
* You can see injection code query into username parameters as show below

![图片](https://user-images.githubusercontent.com/57030243/160414005-c6367ed4-b196-49b4-a9a1-37de92f46d39.png)
![图片](https://user-images.githubusercontent.com/57030243/160416166-fa58058e-e7de-4b82-bbb9-a7aad08f41e4.png)
![图片](https://user-images.githubusercontent.com/57030243/160421624-b17707f0-c9f0-4555-b784-197532e68b97.png)
* You can log in at will through injection(username=test' or 1=1#)

![图片](https://user-images.githubusercontent.com/57030243/160414213-af45c88e-5cee-420f-b910-f5a98165dce0.png)
