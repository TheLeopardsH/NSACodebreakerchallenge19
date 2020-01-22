## Task 1 Description
Submit the APK's SHA256 hash.This will help us search other intelligence sources for connections to users. To test out the app, we also need the registration information their leadership uses to register each client. Analyze the packet capture for this data and submit the registration information for 2 clients (in any order).
There are many challenges that we will need to overcome in order to exploit TerrorTime. The first is that we do not yet have a copy of it. We have learned few details through intelligence sources, but the terrorists have managed to keep the app hidden. It is not publicly available on any App Store. Fortunately, as part of a recent military operation, specialized collection gear was forward deployed near the terrorist's area of operations. This resulted in a trove of collected traffic and we need your help to analyze it. Your first task is to find and extract a copy of the TerrorTime Android Package (APK) file from the packet capture. 


## Write-up
        I am given packet capture(terrortime.pcapng).When I open it in wireshark, I need to look at http traffic and it has terrorTime.apk file and apk developer information.We can export it via File -> Export Objects -> HTTP and save it in some location.Note I uploaded apk file and Developer information here.
![](https://github.com/TheLeopardsH/NSACodebreakerchallenge19/blob/master/Task1/terrorTimewireshark.PNG)
        
In task 1  I have to provide  SHA256 hash and registration information for two clients.So

### Hash of terrorTime.apk:

Command: sha256sum terrorTime.apk
![](https://github.com/TheLeopardsH/NSACodebreakerchallenge19/blob/master/Task1/sha3hash.PNG)

### Registration information is avaialable in README.developer
test1--vhost-1234@terrortime.app:secret1

test2--vhost-1234@terrortime.app:secret2
