### tomcat log

logstash -f logstash-tool-kit/tomcat/catalina.conf
logstash -f logstash-tool-kit/test/grok.conf

reference https://stackoverflow.com/questions/25429377/how-can-i-integrate-tomcat6s-catalina-out-file-with-logstash-elasticsearch