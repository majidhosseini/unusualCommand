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




multiuser of github, gitlab, and local git
add file ~/.ssh/config

and add this parts


Host gitlab.com
    HostName gitlab.com
    User ma3hosseini@gmail.com
    IdentityFile ~/.ssh/me_id_rsa
Host git.pinsvc.net
    HostName git.pinsvc.net
    User majid.hosseini@snapptrip.com
    IdentityFile ~/.ssh/id_rsa
Host github.com
    HostName github.com
    User ma3hosseini@gmail.com
    IdentityFile ~/.ssh/me_id_rsa
