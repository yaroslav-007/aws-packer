
# kitchen-travis test
Packer that create image box that has nginx installed

## pre-requirements

all pre-requirementa to make this work here:
- Linux OS Ubuntu 18.04
- Install **Packer**
	- Download Vagrant from https://www.packer.io/downloads.html
	- Extract the binary file and move/copy it to /usr/local/bin/
	- Check if installed 
		``` packer -v ```
- Create **AWS account**
	- Create sandbox account
    - Generete Access key and secret key
    - Create via console ec2 instance
    - Generate key pairs and added ot on /.ssh/id_rsa


## How to run the code
In the terminal run the following commands:
```
    export AWS_ACCESS_KEY_ID=<ACCESS_KEY>
    export AWS_SECRET_ACCESS_KEY=<SECRET_ACCESS>
    packer build template.json
```