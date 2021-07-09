# errord_devcontainer20210709

vscode-remote-container error container pattern.

## OK pattern

* v0.183.0
![OK image](./img/2021-07-09_164903.png "OK Image")

<details><summary>detail</summary>

```log
[471 ms] Remote-Containers 0.183.0 in VS Code 1.58.0 (2d23c42a936db1c7b3b06f918cde29561cc47cd6).
[470 ms] Start: Resolving Remote
[478 ms] Setting up container for folder or workspace: 
************************************\errord_devcontainer20210709
[481 ms] Start: Check Docker is running
[481 ms] Start: Run: docker version --format {{.Server.APIVersion}}
[968 ms] Server API version: 1.41
[1074 ms] Start: Run: docker-compose version --short
[2321 ms] Start: Run: docker ps -q -a --filter label=com.docker.compose.project=errord_devcontainer20210709 --filter label=com.docker.compose.service=php
[2906 ms] Start: Run: docker inspect --type container b2e695a99e08
[3418 ms] Start: Run: docker-compose -f ************************************\errord_devcontainer20210709\docker-compose.yml config --services
[5347 ms] php
[5347 ms] 
[5347 ms] Start: Run: docker events --format {{json .}} --filter event=start
[5380 ms] Start: Run: docker-compose --project-name errord_devcontainer20210709 -f ************************************\errord_devcontainer20210709\docker-compose.yml up -d
Starting errord_devcontainer20210709_php_1 ... done
[9408 ms] Start: Run: docker ps -q -a --filter label=com.docker.compose.project=errord_devcontainer20210709 --filter label=com.docker.compose.service=php
[9886 ms] Start: Run: docker inspect --type container b2e695a99e08
[10353 ms] Start: Inspecting container
[10354 ms] Start: Run: docker inspect --type container b2e695a99e080d2a92b5d89fd2ef890423f7c16490a7e02cbb9567d21119922d
[10820 ms] Start: Run in container: /bin/sh
[10850 ms] Start: Run in container: uname -m
[12387 ms] x86_64
[12388 ms] 
[12388 ms] Start: Run in container: (cat /etc/os-release || cat /usr/lib/os-release) 2>/dev/null
[12392 ms] PRETTY_NAME="Debian GNU/Linux 10 (buster)"
NAME="Debian GNU/Linux"
VERSION_ID="10"
VERSION="10 (buster)"
VERSION_CODENAME=buster
ID=debian
HOME_URL="https://www.debian.org/"
SUPPORT_URL="https://www.debian.org/support"
BUG_REPORT_URL="https://bugs.debian.org/"
[12393 ms] 
[12394 ms] Start: Run in container: cat /etc/passwd
[12398 ms] Start: Setup shutdown monitor
[12399 ms] Forking shutdown monitor: ****************\.vscode\extensions\ms-vscode-remote.remote-containers-0.183.0\dist\shutdown\shutdownMonitorProcess \\.\pipe\vscode-remote-containers-d96d88a97d3655cce441ebc7f63a3e46929fd455-sock dockerCompose Debug ****************\AppData\Roaming\Code\logs\20210709T135439\exthost7\ms-vscode-remote.remote-containers 1625818994320
[12418 ms] Start: Run in container: test -d /home/vscode/.vscode-server
[12432 ms] 
[12432 ms] 
[12433 ms] Start: Run in container: test -f /var/vscode-server/.patchEtcEnvironmentMarker
[12437 ms] 
[12438 ms] 
[12439 ms] Start: Run in container: test -f /var/vscode-server/.patchEtcProfileMarker
[12446 ms] 
[12446 ms] 
[12446 ms] Start: Run in container: set -o noclobber ; mkdir -p '/home/vscode/.vscode-server/data/Machine' && { > '/home/vscode/.vscode-server/data/Machine/.writeMachineSettingsMarker' ; } 2> /dev/null
[12458 ms] 
[12459 ms] 
[12459 ms] Exit code 2
[12460 ms] Start: Run in container: cat /home/vscode/.vscode-server/data/Machine/settings.json
[12464 ms] {
        "php.validate.executablePath": "/usr/local/bin/php",
        "remote.portsAttributes": {
                "8000": {
                        "label": "Hello Remote World",
                        "onAutoForward": "notify"
                }
        }
}
[12465 ms] 
[12466 ms] Start: Run in container: test -d /home/vscode/.vscode-server/bin/2d23c42a936db1c7b3b06f918cde29561cc47cd6
[12468 ms] 
[12469 ms] 
[12469 ms] Start: Launching Remote-Containers helper.
[12470 ms] Start: Run: gpgconf --list-dir agent-extra-socket
[12499 ms] findLocalWindowsExecutable: Exectuable 'gpgconf' not found on PATH 'C:\WINDOWS\system32;C:\WINDOWS;C:\WINDOWS\System32\Wbem;C:\WINDOWS\System32\WindowsPowerShell\v1.0\;C:\WINDOWS\System32\OpenSSH\;C:\Program Files\dotnet\;C:\Program Files\TortoiseGit\bin;C:\Program Files\Microsoft SQL Server\130\Tools\Binn\;C:\Program Files\Microsoft SQL Server\Client SDK\ODBC\170\Tools\Binn\;C:\Program Files (x86)\Windows Kits\10\Windows Performance Toolkit\;C:\Program Files\Git\cmd;C:\Program Files\nodejs\;C:\Program Files\PowerShell\7-preview\preview;C:\Program Files\Docker\Docker\resources\bin;C:\ProgramData\DockerDesktop\version-bin;****************\AppData\Local\Microsoft\WindowsApps;;****************\AppData\Local\Programs\Microsoft VS Code\bin;****************\.dotnet\tools;****************\AppData\Roaming\npm'.
[12503 ms] userEnvProbe: loginInteractiveShell (default)
[12505 ms] userEnvProbe shell: /bin/bash
[12505 ms] Start: Run in container: /bin/sh
[12508 ms] Start: Run in container: cat <<'EOF-/tmp/vscode-remote-containers-a472e6984bd39a145ffaed2911f3c269fd61d2a0.js' >/tmp/vscode-remote-containers-a472e6984bd39a145ffaed2911f3c269fd61d2a0.js
[12533 ms] Start: Run in container: command -v git >/dev/null 2>&1 && git config --system credential.helper '!f() { /home/vscode/.vscode-server/bin/2d23c42a936db1c7b3b06f918cde29561cc47cd6/node /tmp/vscode-remote-containers-a472e6984bd39a145ffaed2911f3c269fd61d2a0.js $*; }; f' || true
[12575 ms] 
[12576 ms] 
[12576 ms] Start: Run in container: cat <<'EOF-/tmp/vscode-remote-containers-server-a472e6984bd39a145ffaed2911f3c269fd61d2a0.js' >/tmp/vscode-remote-containers-server-a472e6984bd39a145ffaed2911f3c269fd61d2a0.js
[12596 ms] 
[12596 ms] 
[12597 ms] Start: Run in container: /home/vscode/.vscode-server/bin/2d23c42a936db1c7b3b06f918cde29561cc47cd6/node /tmp/vscode-remote-containers-server-a472e6984bd39a145ffaed2911f3c269fd61d2a0.js
[13215 ms] 
[13215 ms] 
[13216 ms] Start: Preparing Extensions
[13216 ms] Start: Run in container: set -o noclobber ; mkdir -p '/home/vscode/.vscode-server/data/Machine' && { > '/home/vscode/.vscode-server/data/Machine/.installExtensionsMarker' ; } 2> /dev/null
[13220 ms] 
[13220 ms] 
[13221 ms] Exit code 2
[13224 ms] Extensions cache, install extensions: MS-CEINTL.vscode-language-pack-ja
[13225 ms] Start: Run in container: test -d /home/vscode/.vscode-server/extensionsCache && ls /home/vscode/.vscode-server/extensionsCache || true
[13259 ms] bmewburn.vscode-intelephense-client-1.7.1
felixfbecker.php-debug-1.16.1
mrmlnc.vscode-apache-1.2.0
ms-ceintl.vscode-language-pack-ja-1.58.7
[13259 ms] 
[13260 ms] Extensions cache, copy to remote: None
[13261 ms] Start: Run in container: for pid in `cd /proc && ls -d [0-9]*`; do { echo $pid ; readlink /proc/$pid/cwd ; readlink /proc/$pid/ns/mnt ; cat /proc/$pid/stat | tr "
[13397 ms] Start: Starting VS Code Server
[13397 ms] Start: Run in container: /home/vscode/.vscode-server/bin/2d23c42a936db1c7b3b06f918cde29561cc47cd6/server.sh --log debug --force-disable-user-env --use-host-proxy --port 0 --extensions-download-dir /home/vscode/.vscode-server/extensionsCache --install-extension MS-CEINTL.vscode-language-pack-ja --start-server
[13520 ms] 

*
* Visual Studio Code Server
*
* Reminder: You may only use this software with Visual Studio family products,
* as described in the license https://aka.ms/vscode-remote/license
*

Extension host agent listening on 39285

[13520 ms] Start: Run in container: echo 39285 >/home/vscode/.vscode-server/data/Machine/.devport
[13527 ms] 
[13527 ms] 
[13527 ms] Port forwarding for container port 39285 starts listening on local port.
[13529 ms] Port forwarding local port 39285 to container port 39285
[13545 ms] Start: Run in container: set -o noclobber ; mkdir -p '/home/vscode/.vscode-server/data/Machine' && { > '/home/vscode/.vscode-server/data/Machine/.onCreateCommandMarker' ; } 2> /dev/null
[13570 ms] 
[13570 ms] 
[13570 ms] Exit code 2
[13571 ms] Start: Run in container: set -o noclobber ; mkdir -p '/home/vscode/.vscode-server/data/Machine' && { > '/home/vscode/.vscode-server/data/Machine/.updateContentCommandMarker' ; } 2> /dev/null
[13591 ms] 
[13591 ms] 
[13591 ms] Exit code 2
[13592 ms] Start: Run in container: set -o noclobber ; mkdir -p '/home/vscode/.vscode-server/data/Machine' && { > '/home/vscode/.vscode-server/data/Machine/.postCreateCommandMarker' ; } 2> /dev/null
[13608 ms] 
[13608 ms] 
[13608 ms] Exit code 2
[13609 ms] Start: Run in container: # Test for /home/vscode/.gitconfig and git
[13618 ms] /home/vscode/.gitconfig exists
[13618 ms] 
[13618 ms] Exit code 1
[13619 ms] Start: Run in container: command -v git >/dev/null 2>&1 && git config --global credential.helper '!f() { /home/vscode/.vscode-server/bin/2d23c42a936db1c7b3b06f918cde29561cc47cd6/node /tmp/vscode-remote-containers-a472e6984bd39a145ffaed2911f3c269fd61d2a0.js $*; }; f' || true
[13695 ms] 
[13696 ms] 
[13696 ms] Start: Run in container: mkdir -p '/home/vscode/.vscode-server/data/Machine' && [ "$(cat '/home/vscode/.vscode-server/data/Machine/.postStartCommandMarker' 2>/dev/null)" != '2021-07-09T08:23:23.3404973Z' ] && echo '2021-07-09T08:23:23.3404973Z' > '/home/vscode/.vscode-server/data/Machine/.postStartCommandMarker'
[13717 ms] 
[13717 ms] 
[13841 ms] [08:23:28] Extension host agent started.
[13865 ms] userEnvProbe PATHs:
Probe:     '/usr/local/share/nvm/current/bin:/usr/local/share/nvm/versions/node/v14.17.3/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/home/vscode/.local/bin'
Container: '/usr/local/share/nvm/current/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin'
[13899 ms] Installing extensions...
[13918 ms] Port forwarding connection from 63088 > 39285 > 39285 in the container.
[13919 ms] Start: Run in container: /home/vscode/.vscode-server/bin/2d23c42a936db1c7b3b06f918cde29561cc47cd6/node -e 
[14257 ms] Extension 'ms-ceintl.vscode-language-pack-ja' v1.58.7 is already installed. Use '--force' option to update to latest version or provide '@<version>' to install a specific version, for example: 'ms-ceintl.vscode-language-pack-ja@1.2.3'.
[14739 ms] Port forwarding connection from 63091 > 39285 > 39285 in the container.
[14740 ms] Start: Run in container: /home/vscode/.vscode-server/bin/2d23c42a936db1c7b3b06f918cde29561cc47cd6/node -e 
[14777 ms] [08:23:29] [::ffff:127.0.0.1][8bdc30a6][ManagementConnection] New connection established.
[15901 ms] [08:23:30] [::ffff:127.0.0.1][572ace38][ExtensionHostConnection] New connection established.
[15932 ms] [08:23:30] [::ffff:127.0.0.1][572ace38][ExtensionHostConnection] <387> Launched Extension Host Process.
```

</details>

## NG pattern

* v0.184.0
![NG image](./img/2021-07-09_165552.png "NG Image")

<details><summary>detail</summary>

```log
[2021-07-09T08:26:12.988Z] Remote-Containers 0.184.0 in VS Code 1.58.0 (2d23c42a936db1c7b3b06f918cde29561cc47cd6).
[2021-07-09T08:26:12.988Z] Start: Resolving Remote
[2021-07-09T08:26:12.992Z] Setting up container for folder or workspace: ************************************\errord_devcontainer20210709
[2021-07-09T08:26:12.994Z] Start: Check Docker is running
[2021-07-09T08:26:12.995Z] Start: Run: docker version --format {{.Server.APIVersion}}
[2021-07-09T08:26:13.471Z] Stop (476 ms): Run: docker version --format {{.Server.APIVersion}}
[2021-07-09T08:26:13.471Z] Server API version: 1.41
[2021-07-09T08:26:13.471Z] Stop (477 ms): Check Docker is running
[2021-07-09T08:26:13.580Z] Start: Run: docker-compose version --short
[2021-07-09T08:26:14.786Z] Stop (1206 ms): Run: docker-compose version --short
[2021-07-09T08:26:14.788Z] Start: Run: docker ps -q -a --filter label=com.docker.compose.project=errord_devcontainer20210709 --filter label=com.docker.compose.service=php
[2021-07-09T08:26:15.309Z] Stop (521 ms): Run: docker ps -q -a --filter label=com.docker.compose.project=errord_devcontainer20210709 --filter label=com.docker.compose.service=php
[2021-07-09T08:26:15.310Z] Start: Run: docker inspect --type container b2e695a99e08
[2021-07-09T08:26:15.807Z] Stop (497 ms): Run: docker inspect --type container b2e695a99e08
[2021-07-09T08:26:15.809Z] Start: Run: docker-compose -f ************************************\errord_devcontainer20210709\docker-compose.yml config
[2021-07-09T08:26:17.530Z] Stop (1721 ms): Run: docker-compose -f ************************************\errord_devcontainer20210709\docker-compose.yml config
[2021-07-09T08:26:17.530Z] 
[2021-07-09T08:26:17.530Z] Traceback (most recent call last):
  File "docker-compose", line 3, in <module>
  File "compose\cli\main.py", line 81, in main
  File "compose\cli\main.py", line 197, in perform_command
  File "compose\metrics\decorator.py", line 18, in wrapper
  File "compose\cli\main.py", line 441, in config
UnicodeEncodeError: 'cp932' codec can't encode character '\U0001f31f' in position 259: illegal multibyte sequence
[6368] Failed to execute script docker-compose

[2021-07-09T08:26:17.530Z] Exit code 4294967295
[2021-07-09T08:26:17.534Z] Command failed: docker-compose -f ************************************\errord_devcontainer20210709\docker-compose.yml config

```

</details>
