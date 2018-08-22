# unusualCommand
Add SSH
$ ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
> Adding your SSH key to the ssh-agent
$ eval "$(ssh-agent -s)"
$ ssh-add ~/.ssh/id_rsa
> copy in clipboard
$ xclip -sel clip < ~/.ssh/id_rsa.pub
> Test yours
# ssh -T [EMAIL]

sudo visudo
[user] ALL=(ALL) NOPASSWD: /usr/bin/openconnect
