# boost-ppa
PPA repository for boost libraries

# Usage

To use this PPA:

```
curl -s --compressed "https://nureva-com.github.io/boost-ppa/KEY.gpg" | gpg --dearmor | sudo tee /usr/share/keyrings/nureva-boost-archive-keyring.gpg
sudo curl -s --compressed -o /etc/apt/sources.list.d/nureva-boost.list "https://nureva-com.github.io/boost-ppa/nureva-boost.list"
sudo apt update
```

# Updating/adding new packages

Put your new .deb files inside the git repo and run `./bin/generate.sh` to
update the files. Then commit and push to repo.