# sample-web-server
テクノロジー（藤原）Node.jsによるサンプルWebサーバ

```
yanyuwende-MacBook-Pro:~ yenyuwen$ cd ~/fujiwara
yanyuwende-MacBook-Pro:fujiwara yenyuwen$ git clone git@github.com:yuwenyen/sample-web-server.git
Cloning into 'sample-web-server'...
remote: Enumerating objects: 7, done.
remote: Counting objects: 100% (7/7), done.
remote: Compressing objects: 100% (5/5), done.
remote: Total 7 (delta 1), reused 5 (delta 1), pack-reused 0
Receiving objects: 100% (7/7), done.
Resolving deltas: 100% (1/1), done.
yanyuwende-MacBook-Pro:fujiwara yenyuwen$ cd sample-web-server
yanyuwende-MacBook-Pro:sample-web-server yenyuwen$ code .
yanyuwende-MacBook-Pro:sample-web-server yenyuwen$ curl --silent --request GET --url https://api.thecatapi.com/v1/images/search
[{"breeds":[],"id":"186","url":"https://cdn2.thecatapi.com/images/186.gif","width":180,"height":180}]yanyuwende-MacBook-Pro:sample-web-server yenyuwen$ 
yanyuwende-MacBook-Pro:sample-web-server yenyuwen$ https://cdn2.thecatapi.com/images/186.gif
-bash: https://cdn2.thecatapi.com/images/186.gif: No such file or directory
yanyuwende-MacBook-Pro:sample-web-server yenyuwen$ 
yanyuwende-MacBook-Pro:sample-web-server yenyuwen$  curl --silent --request GET --url https://api.thecatapi.com/v1/images/search
[{"breeds":[],"categories":[{"id":6,"name":"caturday"}],"id":"5v0","url":"https://cdn2.thecatapi.com/images/5v0.jpg","width":2816,"height":2112}]yanyuwende-MacB-url 'https://api.thecatapi.com/v1/images/search?limit=3'st GET - 
[{"breeds":[],"id":"2oo","url":"https://cdn2.thecatapi.com/images/2oo.gif","width":330,"height":186},{"breeds":[],"id":"3pj","url":"https://cdn2.thecatapi.com/images/3pj.jpg","width":500,"height":334},{"breeds":[],"id":"d67","url":"https://cdn2.thecatapi.com/images/d67.jpg","width":400,"height":294}]yanyuwende-MacBook-Pro:sample-web-server yenyuwen$ 
yanyuwende-MacBook-Pro:sample-web-server yenyuwen$ brew install jq
Updating Homebrew...
^C==> Installing dependencies for jq: oniguruma
==> Installing jq dependency: oniguruma
^C
yanyuwende-MacBook-Pro:sample-web-server yenyuwen$ brew install jq
Updating Homebrew...
==> Installing dependencies for jq: oniguruma
==> Installing jq dependency: oniguruma
==> Downloading https://homebrew.bintray.com/bottles/oniguruma-6.9.2.mojave.bott
^C
yanyuwende-MacBook-Pro:sample-web-server yenyuwen$ brew install jq
==> Installing dependencies for jq: oniguruma
==> Installing jq dependency: oniguruma
==> Downloading https://homebrew.bintray.com/bottles/oniguruma-6.9.2.mojave.bott

curl: (6) Could not resolve host: homebrew.bintray.com
Error: Failed to download resource "oniguruma"
Download failed: https://homebrew.bintray.com/bottles/oniguruma-6.9.2.mojave.bottle.tar.gz
Warning: Bottle installation failed: building from source.
==> Downloading https://github.com/kkos/oniguruma/releases/download/v6.9.2/onig-

curl: (6) Could not resolve host: github.com
Error: An exception occurred within a child process:
  DownloadError: Failed to download resource "oniguruma"
Download failed: https://github.com/kkos/oniguruma/releases/download/v6.9.2/onig-6.9.2.tar.gz

yanyuwende-MacBook-Pro:sample-web-server yenyuwen$ brew install jq

==> Installing dependencies for jq: oniguruma
==> Installing jq dependency: oniguruma
==> Downloading https://homebrew.bintray.com/bottles/oniguruma-6.9.2.mojave.bott

curl: (6) Could not resolve host: homebrew.bintray.com
Error: Failed to download resource "oniguruma"
Download failed: https://homebrew.bintray.com/bottles/oniguruma-6.9.2.mojave.bottle.tar.gz
Warning: Bottle installation failed: building from source.
==> Downloading https://github.com/kkos/oniguruma/releases/download/v6.9.2/onig-

curl: (6) Could not resolve host: github.com
Error: An exception occurred within a child process:
  DownloadError: Failed to download resource "oniguruma"
Download failed: https://github.com/kkos/oniguruma/releases/download/v6.9.2/onig-6.9.2.tar.gz

yanyuwende-MacBook-Pro:sample-web-server yenyuwen$ 
yanyuwende-MacBook-Pro:sample-web-server yenyuwen$ brew cleanup
Warning: Skipping libidn2: most recent version 2.2.0 not installed
Warning: Skipping wget: most recent version 1.20.3_1 not installed
Pruned 0 symbolic links and 2 directories from /usr/local
yanyuwende-MacBook-Pro:sample-web-server yenyuwen$ brew install jq
Updating Homebrew...
==> Auto-updated Homebrew!
Updated 1 tap (homebrew/core).
==> New Formulae
drone-cli                  scala@2.12                 swig@3
==> Updated Formulae
openssl ✔                  go                         paket
anyenv                     godep                      pandoc
aravis                     goofys                     phpmyadmin
armadillo                  grakn                      phpunit
atlantis                   graph-tool                 procs
aws-sdk-cpp                gst-plugins-good           pulumi
bitrise                    helmfile                   pybind11
braid                      hlint                      pyenv
buildifier                 imagemagick                rbspy
calicoctl                  imagemagick@6              scala
certbot                    jdupes                     scalariform
cfn-lint                   jenkins                    scons
chakra                     jenkins-lts                scrcpy
circleci                   jfrog-cli-go               serverless
citus                      jhipster                   ship
cointop                    joplin                     sops
composer                   knot                       sphinx-doc
dependency-check           libev                      telegraf
doctl                      librealsense               terraform
encfs                      libsigc++                  terragrunt
envconsul                  libtorrent-rasterbar       tokei
exiftool                   lmod                       tomcat
firebase-cli               macvim                     topgrade
flow                       mesa                       vultr
fluxctl                    mighttpd2                  webpack
folly                      minio                      whois
gibo                       minio-mc                   wildfly-as
glib                       node-build                 wtf
glooctl                    nomad                      yelp-tools
gmic                       opa                        you-get
==> Deleted Formulae
scala@2.10                               swig@3.04

==> Installing dependencies for jq: oniguruma
==> Installing jq dependency: oniguruma
==> Downloading https://homebrew.bintray.com/bottles/oniguruma-6.9.2.mojave.bott
==> Downloading from https://akamai.bintray.com/c6/c613befafe81da48913ebd1a7eb03
######################################################################## 100.0%
==> Pouring oniguruma-6.9.2.mojave.bottle.tar.gz
🍺  /usr/local/Cellar/oniguruma/6.9.2: 17 files, 1.3MB
==> Installing jq
==> Downloading https://homebrew.bintray.com/bottles/jq-1.6.mojave.bottle.1.tar.
==> Downloading from https://akamai.bintray.com/71/71f0e76c5b22e5088426c971d5e79
######################################################################## 100.0%
==> Pouring jq-1.6.mojave.bottle.1.tar.gz
🍺  /usr/local/Cellar/jq/1.6: 18 files, 1MB
yanyuwende-MacBook-Pro:sample-web-server yenyuwen$ curl --silent --request GET --url 'https://api.thecatapi.com/v1/images/search?limit=3' | jq
[
  {
    "breeds": [],
    "id": "9cv",
    "url": "https://cdn2.thecatapi.com/images/9cv.jpg",
    "width": 600,
    "height": 600
  },
  {
    "breeds": [],
    "id": "sSkPpO5gd",
    "url": "https://cdn2.thecatapi.com/images/sSkPpO5gd.jpg",
    "width": 3024,
    "height": 4032
  },
  {
    "breeds": [],
    "id": "mQvRic06p",
    "url": "https://cdn2.thecatapi.com/images/mQvRic06p.jpg",
    "width": 343,
    "height": 147
  }
]
yanyuwende-MacBook-Pro:sample-web-server yenyuwen$ curl --silent --request GET --url 'https://api.thecatapi.com/v1/images/search?limit=3' > thecat.json
yanyuwende-MacBook-Pro:sample-web-server yenyuwen$ git add .
yanyuwende-MacBook-Pro:sample-web-server yenyuwen$ git commit -m '6/14 課題'
[master a3ce446] 6/14 課題
 1 file changed, 1 insertion(+)
 create mode 100644 thecat.json
yanyuwende-MacBook-Pro:sample-web-server yenyuwen$ git push -u origin master
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 1.04 KiB | 1.04 MiB/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To github.com:yuwenyen/sample-web-server.git
   e137d16..a3ce446  master -> master
Branch 'master' set up to track remote branch 'master' from 'origin'.
yanyuwende-MacBook-Pro:sample-web-server yenyuwen$ cd fujiwara
-bash: cd: fujiwara: No such file or directory
yanyuwende-MacBook-Pro:sample-web-server yenyuwen$ cd ~/fujiwara
yanyuwende-MacBook-Pro:fujiwara yenyuwen$ ls
hello-git		sample-web-server
learning-http-message	simple-web-site
yanyuwende-MacBook-Pro:fujiwara yenyuwen$ cd sample-web-server
yanyuwende-MacBook-Pro:sample-web-server yenyuwen$ code .
yanyuwende-MacBook-Pro:sample-web-server yenyuwen$ mkdir mywebapi
yanyuwende-MacBook-Pro:sample-web-server yenyuwen$ cd mywebapi
yanyuwende-MacBook-Pro:mywebapi yenyuwen$ npm init
This utility will walk you through creating a package.json file.
It only covers the most common items, and tries to guess sensible defaults.

See `npm help json` for definitive documentation on these fields
and exactly what they do.

Use `npm install <pkg>` afterwards to install a package and
save it as a dependency in the package.json file.

Press ^C at any time to quit.
package name: (mywebapi) 
version: (1.0.0) 
description: 
entry point: (index.js) 
test command: 
git repository: 
keywords: 
author: 
license: (ISC) 
About to write to /Users/yenyuwen/Documents/fujiwara/sample-web-server/mywebapi/package.json:

{
  "name": "mywebapi",
  "version": "1.0.0",
  "description": "",
  "main": "index.js",
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1"
  },
  "author": "",
  "license": "ISC"
}


Is this OK? (yes) 
yanyuwende-MacBook-Pro:mywebapi yenyuwen$ nmp install --save express
-bash: nmp: command not found
yanyuwende-MacBook-Pro:mywebapi yenyuwen$ npm install --save express
npm notice created a lockfile as package-lock.json. You should commit this file.
npm WARN mywebapi@1.0.0 No description
npm WARN mywebapi@1.0.0 No repository field.

+ express@4.17.1
added 50 packages from 37 contributors and audited 126 packages in 3.604s
found 0 vulnerabilities

yanyuwende-MacBook-Pro:mywebapi yenyuwen$ node index.js
Listening on port 3000

