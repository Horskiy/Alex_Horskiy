# install gitlab ce
```bash
sudo apt-get update
sudo apt-get install -y curl openssh-server ca-certificates tzdata perl

curl https://packages.gitlab.com/install/repositories/gitlab/gitlab-ce/script.deb.sh | sudo bash


sudo EXTERNAL_URL="https://gitlab.example.com" apt-get install gitlab-ce
sudo EXTERNAL_URL="http://localhost" apt-get install gitlab-ce

# List available versions: apt-cache madison gitlab-ee
# Specifiy version: 
sudo EXTERNAL_URL="https://gitlab.example.com" apt-get install gitlab-ee=16.2.3-ee.0
# Pin the version to limit auto-updates: sudo apt-mark hold gitlab-ee
# Show what packages are held back: sudo apt-mark showhold


```
# My Bad