Apache Tomcat
=====

Install
-----
	curl -s https://raw.githubusercontent.com/oscm/shell/master/os/user/www.sh | bash
	curl -s https://raw.githubusercontent.com/oscm/shell/master/web/tomcat/apache-tomcat.sh | bash

systemd
-----
	curl -s https://raw.githubusercontent.com/oscm/shell/master/web/tomcat/systemctl.sh | bash
	
logrotate
-----
	curl -s https://raw.githubusercontent.com/oscm/shell/master/web/tomcat/logrotate.d/compress | bash
	
Create a test file
-----
	wget -O /srv/apache-tomcat/*/webapps/ROOT/index.jsp https://raw.githubusercontent.com/oscm/shell/master/web/tomcat/webapps/ROOT/index.jsp

Test
-----
	# curl http://localhost:8080/

	<HTML>
	<HEAD>
	<TITLE>HelloWorld!</TITLE>
	</HEAD>
	<BODY>
	<h1>Hello World!</h1>

	</BODY>
	</HTML>

Tomcat 8.5.15
-----
	curl -s https://raw.githubusercontent.com/oscm/shell/master/web/tomcat/8.5/apache-tomcat-8.5.15.sh | bash