# ssl
how to generate ssl request and configure in apache and jboss server



Step-01

#CN=Common Name should be your servername
```
openssl req -x509 -newkey rsa:4096 -keyout apache.key -out apache.crt -days 365 -nodes
```
Step-02
Now take this apache.crt file and upload to godaady server and generate certificate. It will download you two cer files.

Step-03 
provide path of apache.key and two downloaded .cer extension certificate files to apache configuration


### Error
keytool error: java.lang.Exception: Public keys in reply and keystore don't match
