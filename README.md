`ssh-keygen -t rsa -C "otkuth@gmail.com" -f "id_otku"`

`ssh-keygen -t rsa -C "johnyang247@gmail.com" -f "id_yohnjang"`

`cat ~/.ssh/id_otku.pub`

`cat ~/.ssh/id_yohnjang.pub`


`ssh-add -l`

`eval "$(ssh-agent -s)"`

`ssh-add -D`

`ssh-add ~/.ssh/id_rsa`

## Show email and username for local repository

`git config user.name`
`git config user.email`


## Set email and username for local repository

`git config user.name "otku"`
`git config user.email "otkuth@gmail.com"`


`git clone git@github.com-otku:otku/repo_name.git`

## Creating new repository
`git init`

`git remote add origin git@github.com-otku:otku/repo_name.git`



## ~/.ssh/config

`
# OTKU
Host github.com-otku
   HostName github.com
   User git
   IdentityFile ~/.ssh/id_otku

# YOHNJANG
Host github.com-yohnjang   
   HostName github.com
   User git
   IdentityFile ~/.ssh/id_yohnjang

`


