Configure:

Environment Variables:

export GIT_USERNAME=your_username
export GIT_PASSWORD=your_password

git config --global credential.helper store
git config --global user.name $GIT_USERNAME
git config --global user.email your_email@example.com
git config --global user.password $GIT_PASSWORD

if doesn't work, try:
git remote rm origin
git remote add origin https://$GIT_USERNAME:$GIT_PASSWORD@github.com/USERNAME/REPONAME.git
git fetch origin
