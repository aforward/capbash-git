capbash-git
==============

Scripts for installing [git](http://git-scm.com/) and cloning a repository.

# How to Install #

Install capbash first, more details at:
https://github.com/aforward/capbash

```
git clone https://github.com/aforward/capbash YOUR_REPO_ROOT
cd YOUR_REPO_ROOT
./bootstrap
```

Now you can install git into your project

```
./capbash install git
```

# Configurations #

The available configurations include:

```
GIT_BASE_DIR=${GIT_HOME-/var/apps}
GIT_REPO_NAME=${GIT_PROJECT_NAME-samplephp}
GIT_URL=${GIT_URL-https://github.com/aforward/samplephp}
GIT_REMOTE=${PHPAPP_REMOTE-origin}
GIT_BRANCH=${PHPAPP_BRANCH-master}
```


# Deploy to Remote Server #

To push the git script to your server, all you need if the IP or hostname of your server (e.g. 192.167.0.48) and your root password.

```
./capbash deploy <IP> git
```

For example,

```
./capbash deploy 127.0.0.1 git
```
