---
description: NOTE TAKING AND KEEPING OF DETAILED PROCESSES ON PROJECTS
layout: landing
---

# 🏷 PROJECT-NOTES

## Installation and Configuration of Oracle VM VirtualBox on Ubuntu 22.04

Before Oracle VM VirtualBox Installation, Qt and SDL packages are required or recommended for GUI:

The availability check

with CLI:

```
qmake --version #Output: command 'qmake' not found, but can be installed with: sudo apt install qtchooser.
```

with Script:&#x20;

```
if ! test -x /usr/bin/qmake
then
  # The Qt library is missing...
  echo "error: This script requires Qt to be installed."
  exit 1
fi

# The Qt library is installed
...do your thing...

```

Oracle VM VirtualBox for non-GUI or VBoxHeadless Qt and SDL isn't required or recommended.  &#x20;
