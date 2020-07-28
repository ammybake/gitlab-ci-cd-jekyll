# gitlab-ci-cd-jekyll
With Gitlab CI CD , deploying the jekyll static blog to digitalocean vm , you can deploy in any server . no docker no kubernatives simply on vm 
# Dwonload the jekyll git

docker run --rm --volume="$PWD:/srv/jekyll" -it jekyll/jekyll:latest jekyll new blog

type ls in current dir you'll see /blog folder that contain all you need to deploy   
push all the file inside /blog to your gitlab repo  
next make a .gitlab-ci.yml
make sutiable changes accourding to your needs.... dont' forget to make variable in settings > CI CD section .   
next go to  _ config.yaml and insert your website url in url"" section   
just wait and watch the deployment , as simple as it is !! 
