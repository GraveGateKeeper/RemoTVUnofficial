Unofficial Interface For Remo.TV - Remix from https://github.com/theodorechandler1/LetsRobotUnofficial
# RemoTVUnofficial

RemoTVUnofficial is a easy to use interface for connecting your robot to the remo.tv website.
A minimal example looks like:

```python
from remotv_unofficial import RemoTV

def chatEvent(args):
    #Handle chat events here

def controlEvent(args):
    #Handle control events here

r = RemoTV()
r.addOwner("YourRemoUsername")
r.addRobotKey("YourRobotAPIKey")
r.addChannel("YourChannel")
r.addChatHandler(chatEvent)
r.addControlHandler(controlEvent)
while(True):
    r.wait()
```

Installation is a simple as 
```
pip install remotv_unofficial (not yet)
```

For more information including how to get a api key and a channel (server) visit https://remo.tv
or for additional examples and documentation visit https://github.com/onlybrezel/RemoTVUnofficial
