# test-ssh-repo
process :
 1019  git init
 1020  git add README.md
 1021  git commit -m "first commit"
 1022  git branch -M main
 1023  git remote add origin https://github.com/AlexandreSanofi1/test-ssh-repo.git
 1024  git push -u origin main
 1025  git remote add test-ssh-repo git@github.com:AlexandreSanofi1/test-ssh-repo.git
 1026  git remote -v
 1027  git push --set-upstream test-ssh-repo feature/test-78
 1028  vim test2.txt
 1029  cat test2.txt
 1030  git checkout -b feature/test-78
 1031  git add test2.txt\n
 1032  git commit -m "Added test2.txt to feature/test-78"
 1033  git push --set-upstream test-ssh-repo feature/test-78
 1034  git remote -v
