```
- git config --global alias.st status
- git config --global alias.b branch
- git config --global alias.remoteSSHUrl '!f(){ 
  if [ -z "$1" ]; then
    echo "usage: git remoteSSHUrl <repo-name>" >&2
    return 2
  fi
  git remote add origin "git@github.com:Yash-Daxini/$1.git"
}; f'
- git config --global alias.setRemoteSSHUrl '!f(){ 
  if [ -z "$1" ]; then
    echo "usage: git setRemoteSSHUrl <repo-name>" >&2
    return 2
  fi
  git remote set-url origin "git@github.com:Yash-Daxini/$1.git"
}; f'

```
