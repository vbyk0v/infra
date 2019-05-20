ssh-keygen -t rsa -b 4096 -C "username_1@domain_1"

ssh-keygen -t rsa -b 4096 -C "username_2@domain_2"

.ssh/config:

```
Host domain_1
	HostName domain_1
	User username_1
	IdentityFile private_key_1
	
Host domain_2
	HostName domain_2
	User username_2
	IdentityFile private_key_2
```
add local git cert (ubuntu):
```
sudo cp cert.crt /usr/share/ca-certificates/
sudo update-ca-certificates
```
