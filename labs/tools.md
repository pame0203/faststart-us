
#### Lab Tools

#### Objectives
<br>

Install the IBM® Cloud Private command line interface (CLI) cloudctl.  This CLI is used to create, access, and manage ICP clusters.

__NOTICE:__ Some of the following instructions utilize the __'curl'__ command. If curl is not installed on your laptop it must first be installed to complete this lab. 

Scroll to a CLI tool and desired operating system then follow the installation instructions. <br>


----
----

## cloudctl


<img align="left" width="63" height="81" src="/mdimages/mac_logo.png">&nbsp;
### &nbsp;&nbsp;macOS 

<br>
1 - Download the macOS CLI to install:

Replace <ICP IP> with the IP address of the IBM Cloud Private instance from where the CLI will be obtained.

	curl -kLo cloudctl-darwin-amd64-3.1.1-973 https://<ICP IP>:8443/api/cli/cloudctl-darwin-amd64
	
Example file name from the above curl command:

<p align="center">
<img src="/mdimages/cloudctl_file_macos.png">
</p>

2 - Rename the above downloaded file to cloudctl.  

	mv cloudctl-darwin-amd64-3.1.1-973 cloudctl
	

3 - Make the kubectl binary executable.

	chmod +x ./cloudctl


4 -  Move the binary in to your PATH.

	sudo mv ./cloudctl /usr/local/bin/cloudctl


<br><br>

----

<img align="left" width="63" height="81" src="/mdimages/linux.png">&nbsp;
### &nbsp;&nbsp;Linux 

<br>
1 - Download the Linux CLI to install:

Replace <ICP IP> with the IP address of the IBM Cloud Private instance from where the CLI will be obtained.

	curl -kLo cloudctl-linux-amd64-3.1.1-973 https://<ICP IP>:8443/api/cli/cloudctl-linux-amd64
	
Example file name from the above curl command:

<p align="center">
<img src="/mdimages/cloudctl_file_linux.png">
</p>


2 - Rename the above downloaded file to kubectl.  

	mv cloudctl-linux-amd64-3.1.1-973 cloudctl
	

3 - Make the kubectl binary executable.

	chmod +x ./cloudctl


4 - Move the binary in to your PATH.


	sudo mv ./cloudctl /usr/local/bin/cloudctl


<br><br>

----

<img align="left" width="81" height="63" src="/mdimages/windows10_logo.png">&nbsp;
### Windows 

<br>

1 - Download the Windows CLI to install.

Replace <ICP IP> with the IP address of the IBM Cloud Private instance from where the CLI will be obtained.

	curl -kLo cloudctl-win-amd64-3.1.1-973.exe https://<ICP IP>:8443/api/cli/cloudctl-win-amd64.exe
	
Example file name from the above curl command:

<p align="center">
<img src="/mdimages/cloudctl_file_windows.png">
</p>

2 - Run the above file to install the CLI on the Windows system.

3 - Add the binary in to your PATH.

---

<br><br>

#### Verify the CLI is installed

From a terminal or command prompt enter:

	kubectl version
	

Example output:

<p align="center">
<img src="/mdimages/cloudctl_verify.png">
</p>

----
----


## docker


<img align="left" width="63" height="81" src="/mdimages/mac_logo.png">&nbsp;
### &nbsp;&nbsp;macOS 

<br>

Click this [link](https://docs.docker.com/docker-for-mac/install/) and follow the 
offical docker instructions.


<br><br>

----

<img align="left" width="63" height="81" src="/mdimages/linux.png">&nbsp;
### &nbsp;&nbsp;Linux 

<br>

* Centos - 
Click this [link](https://docs.docker.com/install/linux/docker-ce/centos/) and follow the 
offical docker instructions.

* Debian - 
Click this [link](https://docs.docker.com/install/linux/docker-ce/debian/) and follow the 
offical docker instructions.

* Fedora - 
Click this [link](https://docs.docker.com/install/linux/docker-ce/fedora/) and follow the 
offical docker instructions.

* Ubuntu - 
Click this [link](https://docs.docker.com/install/linux/docker-ce/ubuntu/) and follow the 
offical docker instructions.



<br><br>

----

<img align="left" width="81" height="63" src="/mdimages/windows10_logo.png">&nbsp;
### Windows 

<br>

Click this [link](https://docs.docker.com/docker-for-windows/install/) and follow the 
official docker instructions.



<br><br>

---

## Verify docker CLI is installed

From a terminal or command prompt enter:

	docker version
	

Example output:

<p align="center">
<img src="/mdimages/docker_verify.png">
</p>

----
----

## kubectl


<img align="left" width="63" height="81" src="/mdimages/mac_logo.png">&nbsp;
### &nbsp;&nbsp;macOS 

<br>
1 - Download the macOS CLI to install:

Replace <ICP IP> with the IP address of the IBM Cloud Private instance from where the CLI will be obtained.

	curl -kLo kubectl-darwin-amd64-v1.11.1 https://<ICP IP>:8443/api/cli/kubectl-darwin-amd64
	
Example file name from the above curl command:

<p align="center">
<img src="/mdimages/kubectl_file_macos.png">
</p>

2 - Rename the above downloaded file to kubectl.  

	mv kubectl-darwin-amd64-v1.11.1 kubectl
	

3 - Make the kubectl binary executable.

	chmod +x ./kubectl


4 -  Move the binary in to your PATH.

	sudo mv ./kubectl /usr/local/bin/kubectl


<br><br>

----

<img align="left" width="63" height="81" src="/mdimages/linux.png">&nbsp;
### &nbsp;&nbsp;Linux 

<br>
1 - Download the Linux CLI to install:

Replace <ICP IP> with the IP address of the IBM Cloud Private instance from where the CLI will be obtained.

	curl -kLo kubectl-linux-amd64-v1.11.1 https://<ICP IP>:8443/api/cli/kubectl-linux-amd64
	
Example file name from the above curl command:

<p align="center">
<img src="/mdimages/kubectl_file_linux.png">
</p>


2 - Rename the above downloaded file to kubectl.  

	mv kubectl-linux-amd64-v1.11.1 kubectl
	

3 - Make the kubectl binary executable.

	chmod +x ./kubectl


4 - Move the binary in to your PATH.

	sudo mv ./kubectl /usr/local/bin/kubectl


<br><br>

----

<img align="left" width="81" height="63" src="/mdimages/windows10_logo.png">&nbsp;
### Windows 

<br>

1 - Download the Windows CLI to install.

Replace <ICP IP> with the IP address of the IBM Cloud Private instance from where the CLI will be obtained.

	curl -kLo kubectl-win-amd64-v1.11.1.exe https://<ICP IP>:8443/api/cli/kubectl-win-amd64.exe
	
Example file name from the above curl command:

<p align="center">
<img src="/mdimages/kubectl_file_windows.png">
</p>

2 - Run the above file to install the CLI on the Windows system.

3 - Add the binary in to your PATH.

---

<br><br>

## Verify the CLI is installed

From a terminal or command prompt enter:

	kubectl version
	

Example output:

<p align="center">
<img src="/mdimages/k8_verify.png">
</p>

Once logged in an authenticated with a kubernetes cluster the error portion of the above message will not be shown.

----
----

#### Hint Lab Tools

No hint available for this lab.

----
----

#### Answer Lab Tools

Ensure CLI tools are installed.


> Confirm Tools complete


----
----