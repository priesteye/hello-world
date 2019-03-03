#How to setup heroku-cli on my arm smartphone using Termux

0. apt install wget git proot nodejs nodejs-dev
1. termux-chroot
2. cd /
3. wget https://cli-assets.heroku.com/branches/stable/heroku-linux-arm.tar.gz
4. mkdir -p /usr/local/lib /usr/local/bin
5. tar -xvzf heroku-linux-arm.tar.gz -C /usr/local/lib
6. ln -s /usr/local/lib/heroku/bin/heroku /usr/local/bin/heroku
7. /usr/local/lib/heroku/install
8. cd /home/.local/share/heroku/cli/lib
9. mv node node_broken
10. ln -s /usr/bin/node ./node
11. congratulations
