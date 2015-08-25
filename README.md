# web2py 설치

$sudo wget http://www.web2py.com/examples/static/web2py_src.zip

# web2py 실행

$sudo unzip web2py_src.zip  
cd web2py  
sudo python web2py.py

# pc에서 web2py admin page 접속하는 방법  
  
새로운 인증서를 만들어준다.  
1. openssl genrsa -out server.key 2048  
2. openssl req -new -key server.key -out server.csr  

![images !](images.jpg)
3. openssl x509 -req -days 365 -in server.csr -signkey server.key -out server.crt  

  

