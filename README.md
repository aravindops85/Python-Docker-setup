# Python-Docker-setup
Python script which will convert json files to xml files, encrypt and transfer it in a remote location.

Environment:
Python, Docker

Description:
Solution should be prepared as two Docker images, 1st to send files, and 2nd to receive them.
Deployment of these containers should be automated using docker-compose or shell script.

Python script on container A:
1. convert all json files to xml 
2. encrypt the files
3. Transfer it to a remote location (container B)

Python script on container B:
1. Receive files
2. Decrypt and store files

So, in other words, pipeline should look like:
Json -> XML -> encryption -> transfer -> decryption -> XML

Acceptance criteria:
Any given Json putted to container A appears in XML form on container B using mentioned pipeline.
