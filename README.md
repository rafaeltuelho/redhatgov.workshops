# Getting Started

To use this project, you'll need (at minimum):

- Python 2 >=2.7.9 or Python 3 >=3.4

## Install

#### GNU/Linux, or macOS

```sh
git clone https://github.com:rafaeltuelho/redhatgov.workshops
cd redhatgov.workshops
```

##### No `git`? No problem!

```sh
DIRPATH="${HOME}/Downloads/redhatgov.workshops"; GITUSER="RedHatGov"
GITREPO="https://github.com/${GITUSER}/redhatgov.workshops/archive/master.zip"
ARCHIVE="$(printf "%s" "${GITREPO##*/}")"

# Download and extract
wget $GITREPO \
&& temp="$(mktemp -d)" \
&& unzip -d $temp $ARCHIVE \
&& mkdir -p $DIRPATH \
&& mv $temp/*/* $DIRPATH \
&& rm -rf $temp $ARCHIVE \
&& cd $DIRPATH \
&& unset DIRPATH GITUSER GITREPO ARCHIVE temp
```
