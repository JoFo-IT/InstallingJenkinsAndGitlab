# Installing Jenkins and GitLab
How to installing Jenkins and GitLab on the same Server

## Instaling GitLab


Install necessary dependencies

```
sudo apt-get update
sudo apt-get install -y curl openssh-server ca-certificates tzdata perl
```

Install Postix
 
```
sudo apt-get install -y postfix
```

![alt text](postfix.png)

Downlod install script

```
wget https://packages.gitlab.com/install/repositories/gitlab/gitlab-ee/script.deb.sh
```

Run install script

```
sudo bash script.deb.sh
```

Set external URL and install GitLab

```
sudo EXTERNAL_URL="https://[IP / Domain]" apt-get install gitlab-ee
```

Stop GitLap

```
sudo gitlab-ctl stop
```

Edit config

```
sudo nano /etc/gitlab/gitlab.rb
```

Change port 8080 to 8081

- 
- 
- 
- 

Reconfig GitLab

```
sudo gitlab-ctl reconfigure
```

Restart GitLab

```
sudo gitlab-ctl rerestartboot
```


### Jenkins




# Links
## Jenkins
- [Jenkins](https://www.jenkins.io/)
- [Linux - Jenkins](https://www.jenkins.io/doc/book/installing/linux/)

## GitLab
- [GitLab](https://about.gitlab.com/)
- [Recommended installation](https://about.gitlab.com/install/#ubuntu)
- [Configuration options](https://docs.gitlab.com/omnibus/settings/configuration.html)
