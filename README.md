# SixArm.com » Git » gitconfig for user, alias, color, branch, etc. 

Git configruation settings for our git users, command aliases, 
syntax coloring, branch management, and merge strategies.

## Required

Customize the gitconfig file sections for user:

    [user]
      email = sixarm@sixarm.com
      name = SixArm

Customize the gitconfig file section for GitHub, if you use it:

    [github]
      user = sixarm
      token = sixarm-token


## Recommended

Tell git-branch and git-checkout to setup new branches so that git-pull
will appropriately merge from that remote branch. Without this, you will 
have to add --track to your branch command or manually merge remote
tracking branches with "fetch" and then "merge".

  git config --global branch.autosetupmerge true


## Suggested

When we install Git, we can also install git tab completion settings.

To install git tab completion, we go to the git soure code directory then run:

  echo "source ./contrib/completion/git-completion.bash" >> /etc/bash.bashrc


## Git GUI apps

Read http://git.or.cz/gitwiki/InterfacesFrontendsAndTools

Best is http://cola.tuxfamily.org/

download http://cola.tuxfamily.org/releases/

make prefix=/usr install
