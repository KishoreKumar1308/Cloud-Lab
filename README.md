# Cloud Lab Work-1
## Installing Docker
Docker is used as a container for buliding applications. Instead of installing the entire OS, we can install only the required files.

## Steps:

1. Install an Linux OS in VirtualBox.
2. Update the packages.
3. Install net-tools and ssh.
4. Find the IP of the guest using ifconfig
5. In the VirtualBox Setting for this OS, Go to Network -> Advanced -> Port Forwarding, Give Host port as 20022, Guest IP found from ifconfig and Guest port as 22.
Save the changes.
6. In host machine, Open Command prompt.
7. Type ssh linux-username@127.0.0.1 -p 20022.
8. Grant access if asked and type the guest linux OS password.
9. Create a simple HelloWorld program in the language of your Choice. (I am using Golang)
10. Build the program(create compiled executable file).
11. To containerize the file, we need to install Docker.
12. Go to https://docs.docker.com/engine/install/ubuntu/ and add docker repository to the Ubuntu OS and Install Docker
13. Open a TextEditor
14. Type: from golang:latest, copy helloworld.go .,cmd go run helloworld.go, Save the file as Dockefile
15. In CMD type sudo docker build -t test:1
16. If you run the docker file using sudo docker run test:1, it will give the result of the program even if we remove the golang from our OS. 
