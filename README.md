# AWS Nodjs and Nignx assinment 
## Steps
1.First Install EC2 Instance in AWS.

2.Update EC2 using "yum update command".

3.Install nodejs using "yum install nodejs".

4.Create a js file "vi <file_name>.js"

5.Write js code

"#!/usr/bin/env nodejs

var http = require('http');

http.createServer(function (req, res) {

  res.writeHead(200, {'Content-Type': 'text/plain'});
  
  res.end('Hello World\n');
  
}).listen(8080, 'localhost');

console.log('Server running at http://localhost:8080/');"

6.Install nginx "yum install nginx"

7.Edit location in nginx.conf file "vi /etc/nginx/nginx.conf"

8.proxy_pass http://127.0.0.1:8080;

9.Start server "systemctl start nginx"

10.Now run js file "node <file_name>.js"
