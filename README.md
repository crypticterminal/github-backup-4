# github-backup

// TODO(hbt) ENHANCE update description
Command-line tool to backup data from github


## Copies 

* user and organization repositories (with submodules)
* forks
* starred repositories (cloned)
* watched  repositories (cloned)
* issues (into a JSON file per repository)
* wiki (cloned)
* gists (cloned)
* starred gists (cloned)


## Installation

```
# compatible with latest versions but if you run into issues. This is the official version
rvm use ruby-1.9.3-p547
ruby -v

# compatible with latest bundle but this is the official 
gem install bundle:1.0.0
bundle -v 

git clone git@github.com:hbt/github-backup.git
cd github-backup
bundle

./bin/github-backup -h

```


// TODO(hbt) ENHANCE update usage
## Usage

Usage: github-backup -u [username] -o [dir]
e.g
github-backup -u hbt -o /tmp

    -u, --username USERNAME          *Required: GitHub username
    -o, --output-dir DIR             *Required: Backup directory
    -p, --password PASSWORD          Optional: GitHub password. Required for private repos
    -r, --repository-name NAME       Optional: limit to this repository name
    -O, --organization NAME	          Optional: Organization name to use for fetching repositories, instead of the user
    -f, --forks                      Optional: fetch all forks
    -b, --init-branches              Optional: init all branches
    -i, --dump-issues                Optional: dump all issues
    -w, --wiki                       Optional: dump wiki
    -C, --compress                   Optional: run gc to compress git repo
    -v, --version                    Displays current version
    -h, --help                       Displays this screen


## Copyright

Copyright (c) 2012 hbt. See LICENSE.txt for
further details.

