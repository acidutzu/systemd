
#### copy pythonhttp.service in /lib/systemd/system and sudo chmod 644 the file
```
sudo cp pythonhttp.service /lib/systemd/system/ && chmod 644 pythonhttp.service
```
#### copy files from the start-stop-scripts folder into /usr/local/bin and sudo chmod +x them
```
cd start-stop-scripts
sudo cp pythonhttp-start.sh pythonhttp-stop.sh /usr/local/bin/ && chmod +x pythonhttp-start.sh pythonhttp-stop.sh
```

#### run sudo systemctl enable pythonhttp
```
sudo systemctl enable pythonhttp
```
#### run the service
```
sudo systemctl start pythonhttp
```
