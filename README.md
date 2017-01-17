# codespace-chef-vagrant


Provision Chef Codespace by School of Devops using Vagrant and Virtualbox


## Install Virtualbox and Vagrant


## Download the Codespace Vagrant Image

Download the box from the following URI

https://s3.ap-south-1.amazonaws.com/docker-boxes/ubuntu1604-22.box


## Import Codespace box with Vagrant

Change into the directory where you have downloaded the above box

```
vagrant box add codespace-chef ubuntu1604-22.box

```

Validate

```
vagrant box list
```

Expected Output

```
[output]
codespace-chef (virtualbox, 0)
```


## Clone the Repo to provision Codespace for Chef

```
git clone git@github.com:schoolofdevops/codespace-chef-vagrant.git

```

Alternately you could download the repo from the following URI

 https://github.com/schoolofdevops/codespace-chef-vagrant


Change into the **codespace-chef-vagrant**  created by above command

```
cd  codespace-chef-vagrant

```

## Bring up the Environment with Vagrant and Log into to it

```
vagrant up

vagrant ssh
```

Once the VM environment is up, validate you are able to access Codespaces  for Chef by visiting following URL

http://192.168.51.10:8000

Login : devops
Pass  : codespaces


In addition to the Codespaces IDE, the environment would container following hosts,


| Hostname     | IP Address     |
| :------------- | :------------- |
| node1       | 172.18.0.2     |
| node2       | 172.18.0.3     |
| node3       | 172.18.0.4     |
| node4       | 172.18.0.5     |
