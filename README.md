# COMP6331_STUDY_NOTE

for mqtt, create a pw.txt in the current directory

enter
```
(username:password)
student:33102023
```

Then in command prompt, switch to the directory:
Run
```
mosquitto_passwd -U pw.txt
```
Then the password will be encrypted

in the mosquitto.conf
Add:
```
allow_anonymous false
listener 1883
password_file C:\Program Files\mosquitto\pw.txt
```

restart the service and authentication will be up
