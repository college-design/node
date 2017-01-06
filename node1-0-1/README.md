# Node.js������һ��Ӧ��
1 **���� required ģ�飺���ǿ���ʹ�� require ָ�������� Node.js ģ�顣**
2 **���������������������Լ����ͻ��˵����������� Apache ��Nginx �� HTTP ��������**
3 **������������Ӧ���� �����������״������ͻ��˿���ʹ����������ն˷��� HTTP ���󣬷�������������󷵻���Ӧ���ݡ�**
-----------------
## ����һ������ required ģ��
```var http = require("http");```
## �����������������
```
var http = require('http');

http.createServer(function (request, response) {

	// ���� HTTP ͷ�� 
	// HTTP ״ֵ̬: 200 : OK
	// ��������: text/plain
	response.writeHead(200, {'Content-Type': 'text/plain'});

	// ������Ӧ���� "Hello World"
	response.end('Hello World\n');
}).listen(8888);

// �ն˴�ӡ������Ϣ
console.log('Server running at http://127.0.0.1:8888/');
```
Ȼ����node����ִ�к󣬷��������������������```http://127.0.0.1:8888/```