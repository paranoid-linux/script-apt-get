# Script Apt Get
[heading__top]:
  #script-apt-get
  "&#x2B06; Logs `install` and `update` actions for `apt-get` via `script`"


Logs `install` and `update` actions for `apt-get` via `script`


## [![Byte size of Script Apt Get][badge__main__script_apt_get__source_code]][script_apt_get__main__source_code] [![Open Issues][badge__issues__script_apt_get]][issues__script_apt_get] [![Open Pull Requests][badge__pull_requests__script_apt_get]][pull_requests__script_apt_get] [![Latest commits][badge__commits__script_apt_get__main]][commits__script_apt_get__main] 


------


- [:arrow_up: Top of Document][heading__top]

- [:building_construction: Requirements][heading__requirements]

- [:zap: Quick Start][heading__quick_start]

- [&#x1F9F0; Usage][heading__usage]

- [&#x1F5D2; Notes][heading__notes]

- [:chart_with_upwards_trend: Contributing][heading__contributing]

  - [:trident: Forking][heading__forking]
  - [:currency_exchange: Sponsor][heading__sponsor]

- [:card_index: Attribution][heading__attribution]

- [:balance_scale: Licensing][heading__license]


------



## Requirements
[heading__requirements]:
  #requirements
  "&#x1F3D7; Prerequisites and/or dependencies that this project needs to function properly"


Prerequisites and/or dependencies that this project needs to function properly


- Debian derived distribution

- Sudo or Root permissions


______


## Quick Start
[heading__quick_start]:
  #quick-start
  "&#9889; Perhaps as easy as one, 2.0,..."


Clone this project...


```Bash
mkdir -vp ~/git/hub/paranoid-linux

cd ~/git/hub/paranoid-linux

git clone git@github.com:paranoid-linux/script-apt-get.git
```


Install via symbolic link...


```Bash
cd ~/git/hub/paranoid-linux/script-apt-get

./linked-install.sh
```


Update in the future with Git...


```Bash
cd ~/git/hub/paranoid-linux/script-apt-get

git pull origin main
```


______


## Usage
[heading__usage]:
  #usage
  "&#x1F9F0;"


Install a package with `apt-get`...


```Bash
sudo script-apt-get install vim
```


... Above command will generate a log file at a path similar to...


```
~/Documents/logs/apt-get/install/20200915__vim.script
```


Or upgrade installed packages with `apt-get`...


```Bash
sudo script-apt-get upgrade
```


... Above command will write a log file to a path similar to...


```
~/Documents/logs/apt-get/upgrade/20200915.script
```


______


## Notes
[heading__notes]:
  #notes
  "&#x1F5D2; Additional things to keep in mind when developing"


This repository may not be feature complete and/or fully functional, Pull Requests that add features or fix bugs are certainly welcomed.


------


To customize where log files are saved set the `_log_dir` environment variable per command...


```Bash
_log_dir="${HOME}/script-logs" script-apt-get upgrade
```


... or via `configuration.sh` file, eg...


```Bash
tee -a ~/git/hub/paranoid-linux/script-apt-get/configurations.sh <<'EOF'
_log_dir="${HOME}/script-logs" script-apt-get upgrade
EOF
```


______


## Contributing
[heading__contributing]:
  #contributing
  "&#x1F4C8; Options for contributing to script-apt-get and paranoid-linux"


Options for contributing to script-apt-get and paranoid-linux


------


### Forking
[heading__forking]:
  #forking
  "&#x1F531; Tips for forking script-apt-get"


Start making a [Fork][script_apt_get__fork_it] of this repository to an account that you have write permissions for.


- Add remote for fork URL. The URL syntax is _`git@github.com:<NAME>/<REPO>.git`_...


```Bash
cd ~/git/hub/paranoid-linux/script-apt-get

git remote add fork git@github.com:<NAME>/script-apt-get.git
```


- Commit your changes and push to your fork, eg. to fix an issue...


```Bash
cd ~/git/hub/paranoid-linux/script-apt-get


git commit -F- <<'EOF'
:bug: Fixes #42 Issue


**Edits**


- `<SCRIPT-NAME>` script, fixes some bug reported in issue
EOF


git push fork main
```


> Note, the `-u` option may be used to set `fork` as the default remote, eg. _`git push fork main`_ however, this will also default the `fork` remote for pulling from too! Meaning that pulling updates from `origin` must be done explicitly, eg. _`git pull origin main`_


- Then on GitHub submit a Pull Request through the Web-UI, the URL syntax is _`https://github.com/<NAME>/<REPO>/pull/new/<BRANCH>`_


> Note; to decrease the chances of your Pull Request needing modifications before being accepted, please check the [dot-github](https://github.com/paranoid-linux/.github) repository for detailed contributing guidelines.


------


### Sponsor
  [heading__sponsor]:
  #sponsor
  "&#x1F4B1; Options for financially supporting paranoid-linux that maintains script-apt-get"


Thanks for even considering it!


With [![sponsor__shields_io__liberapay]][sponsor__link__liberapay] you may sponsor paranoid-linux on a repeating basis.


Regardless of if you're able to financially support projects such as `script-apt-get` that `paranoid-linux` maintains, please consider sharing projects that are useful with others, because one of the goals of maintaining Open Source repositories is to provide value to the community.


______


## Attribution
[heading__attribution]:
  #attribution
  "&#x1F4C7; Resources that where helpful in building this project so far."


- [GitHub -- `github-utilities/make-readme`](https://github.com/github-utilities/make-readme)


______


## License
[heading__license]:
  #license
  "&#x2696; Legal side of Open Source"


```
Logs `install` and `update` actions for `apt-get` via `script`
Copyright (C) 2020 S0AndS0

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU Affero General Public License as published
by the Free Software Foundation, version 3 of the License.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU Affero General Public License for more details.

You should have received a copy of the GNU Affero General Public License
along with this program.  If not, see <https://www.gnu.org/licenses/>.

```


For further details review full length version of [AGPL-3.0][branch__current__license] License.



[branch__current__license]:
  /LICENSE
  "&#x2696; Full length version of AGPL-3.0 License"


[badge__commits__script_apt_get__main]:
  https://img.shields.io/github/last-commit/paranoid-linux/script-apt-get/main.svg

[commits__script_apt_get__main]:
  https://github.com/paranoid-linux/script-apt-get/commits/main
  "&#x1F4DD; History of changes on this branch"


[script_apt_get__community]:
  https://github.com/paranoid-linux/script-apt-get/community
  "&#x1F331; Dedicated to functioning code"


[issues__script_apt_get]:
  https://github.com/paranoid-linux/script-apt-get/issues
  "&#x2622; Search for and _bump_ existing issues or open new issues for project maintainer to address."

[script_apt_get__fork_it]:
  https://github.com/paranoid-linux/script-apt-get/
  "&#x1F531; Fork it!"

[pull_requests__script_apt_get]:
  https://github.com/paranoid-linux/script-apt-get/pulls
  "&#x1F3D7; Pull Request friendly, though please check the Community guidelines"

[script_apt_get__main__source_code]:
  https://github.com/paranoid-linux/script-apt-get/
  "&#x2328; Project source!"

[badge__issues__script_apt_get]:
  https://img.shields.io/github/issues/paranoid-linux/script-apt-get.svg

[badge__pull_requests__script_apt_get]:
  https://img.shields.io/github/issues-pr/paranoid-linux/script-apt-get.svg

[badge__main__script_apt_get__source_code]:
  https://img.shields.io/github/repo-size/paranoid-linux/script-apt-get






[sponsor__shields_io__liberapay]:
  https://img.shields.io/static/v1?logo=liberapay&label=Sponsor&message=paranoid-linux

[sponsor__link__liberapay]:
  https://liberapay.com/paranoid-linux
  "&#x1F4B1; Sponsor developments and projects that paranoid-linux maintains via Liberapay"

