# AWS Nodjs and Nginx assinment 
## Steps
1.First Install EC2 Instance in AWS.

2.Update EC2 using "yum update command".

3.Install nodejs using "yum install nodejs".

4.Create a js file "vi <file_name>.js"

5.Write js code

![Screenshot (39)](https://user-images.githubusercontent.com/62141340/117262635-1ad98d00-ae6f-11eb-8888-604a23724b18.png)
6.Install nginx "yum install nginx"

7.Edit location in nginx.conf file "vi /etc/nginx/nginx.conf"

![Screenshot (40)](https://user-images.githubusercontent.com/62141340/117262875-5411fd00-ae6f-11eb-8b5a-040e4b6dc52d.png)

8.proxy_pass http://127.0.0.1:8080;

9.Start server "systemctl start nginx"

10.Now run js file "node <file_name>.js"

