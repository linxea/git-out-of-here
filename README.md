## TODO

### 0. Authenticate Git

1. Using HTTPS

- \$ git remote add origin https://username:password@github.com/linxea/git-out-of-here.git

2. Or using SSH

- Refer to https://help.github.com/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent/

  - \$ ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
  - $eval "$(ssh-agent -s)"
  - \$ ssh-add -K ~/.ssh/id_rsa
  - \$ pbcopy < ~/.ssh/id_rsa.pub

- Add SSH key into Github
  https://help.github.com/articles/adding-a-new-ssh-key-to-your-github-account/

### 1. Create a repo

### 2. Clone to local machine using `git clone`

### 3. Demo git commmands:

- // add /doc folder
- // add index.html in /doc
- \$ git add index.html
- \$ git commit -m "Add index.html with typo"
- \$ git commit --amend # to fix typo
- \$ git push origin master
- // hop over to Github setting to enable Github page
- // change text in index.html
- \$ git add .
- \$ git commit -m "Fix one more thing"
- \$ git push origin master
- // checkout yourname.github.io/git-out-of-here

### 4. If we have more time, demo git hf commands:

- \$ git hf init
- \$ git hf feature start add-new-feature
- // add new change
- \$ git add .
- \$ git commit -m "Add new changes with hf"
- \$ git hf push
- \$ git hf release start production-1.0.0
- \$ git hf release finish production-1.0.0
- // hop over to github repo to see magicccc
