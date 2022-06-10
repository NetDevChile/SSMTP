# SSMTP
Is a Send-Only SendMail Service Installed by APT 

``` 
$ sudo apt update
```

################### instalar SSMTP ########################

``` 
$ sudo apt install ssmtp
```

################# Configurar ssmtp ###############

$ nano /etc/ssmtp/ssmtp.conf

################ ssmtp.conf  ###############

root=site-alarm@netdev.cl
mailhub=mail.netdev.cl:587
AuthUser=site-alarm@netdev.cl
AuthPass=password
AuthMetod=LOGIN
UserSTARTTLS=YES
FromLineOverride=YES
UserTLS=YES
useTLSCert=YES

############### revaliases #################

nut:site-alarm@netdev.cl:mail.netdev.cl:587
