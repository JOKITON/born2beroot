# Born2beroot
Self-made step by step guide to start and finish "born2beroot" project.


Guidelines:
  - We have to make our first virtual machine using VirtualBox with specific instructions. So, when you finish this project you will be able to set up your own operating system using strict rules.

  - The use of VirtualBox is mandatory, you only have to deliver a file named "signature.txt" at the roof of your repository. You must paste in the .txt file the signature of the virtual machine.


  - Mandatory Part:
This projects aim is to create your own first server with some rules:

[We have to take into account that as our only goal is to create a server, we won't need any graphical interface or any other services/tools that are not useful.]

We have to choose as our enviroment the most recent version of Debian, we can also use CentOS, but we are told that Debian is easier to understand if it is our first time working with these enviroments and goals.

-------------------------------------------------------------------ASSIGNMENT------------------------------------------------------------------------------

We need to create at least two encrypted partitions with Logic Volume Manager, we have an example down:
![LogicVolumeManager_born2beroot](https://user-images.githubusercontent.com/99480973/168657734-bc4e0f42-4bfe-4f6a-9363-04c2523ab988.png)


SSH service will only be executed through port number: 4242.
Due to security, it will be not possible to connect through SSH as root.

We have to configure our system with UFW firewall, only letting enabled the port number: 4242.

The hostname of the virtual machine needs to be your login finished with "42", for example: "jaizpuru42".

You have to apply a strong password policy.
