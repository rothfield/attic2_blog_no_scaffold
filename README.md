# Steps

# New rails app, no scaffold, minimal
rails new blog_no_scaffold --skip-git --skip-keeps --skip-action-mailer --skip-action-mailbox --skip-action-text --skip-active-job --skip-active-storage --skip-javascript --skip-hotwire --skip-jbuilder --skip-test --skip-system-test -skip-bootsnap --skip-bundle

# create github repo
gh repo  create

git init

# initial commit
git add .gitignore ; git commit -m "ignore vendor tmp log sqlite3 "

git push --set-upstream origin main

# setup slim as template engine

bundle add html2slim slim-rails rubocop
bundle --binstubs

