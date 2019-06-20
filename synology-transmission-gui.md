## Setting up Transmission on Synology



It would be preferred to install Transmission proper instead of using Download Station. One method is using the community repo.



#### Add Syno Community Repo

`Package Center` > `Settings` > `Package Sources` > `Add` >

```markdown
Name:      SynoCommunity
Location:  http://packages.synocommunity.com/
```



### Install Transmission

Search for Transmission (developer `Safihre`)
Start the service. 
You can connect to the server via web browser, (Your Server IP):9091/transmission/web/
Or install Transmission GUI


### Install Transmission GUI

- Download Link: https://sourceforge.net/projects/transgui
- Source: https://github.com/transmission-remote-gui/transgui


### Configure Transmisison GUI

`File` > `Torrent` > `Connect to Transmission` > `Manage Connections…`

| Application             | Protocol / Port  |
| ----------------------- | ---------------- |
| Connection name         | Local Host       |
| Remote host             | (Your Server IP) |
| Port                    | 9091             |
| Authentication required | Check            |
| User name               | (Your username)  |
| Password                | (Your password)  |



I forgot how to configure the watch directory.

You might need to ssh into Synology to manually set the config file?



`Tools` > `Transmission Options…`



`Tools` > `Application Options…`
