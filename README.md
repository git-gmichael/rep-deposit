---
description: NOTE TAKING AND KEEPING OF DETAILED PROCESSES ON PROJECTS
layout: landing
---

# 🏷 PROJECT-NOTES

## Installation and Configuration of Oracle VM VirtualBox on Ubuntu 22.04

Before Oracle VM VirtualBox Installation, Qt and SDL packages are required or recommended for GUI:

Qt and SDL isn't required or recommended for Oracle VM VirtualBox non-GUI or VBoxHeadless platform users.

Qt Availability check with Script-test:

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

with Script-dpkg:&#x20;

```
if ! dpkg-query -s qtchooser
then
  # The Qt library is missing...
  echo "error: This script requires Qt to be installed."
  exit 1
fi

# The Qt library is installed
...do your thing...
```

Qt Version Check:

```
qmake --version 
# Output: command 'qmake' not found,but can be installed with:
sudo apt install qtchooser
# after qtchooser installation, issue again,
qmake --version # Output: could not exec '/usr/lib/qt5/bin/qmake': No such file or directory
whereis qmake # Output: qmake: /usr/bin/qmake
whereis qtchooser
# Output: qtchooser: /usr/bin/qtchooser /usr/lib/x86_64-linux-gnu/qtchooser /usr/share/qtchooser /usr/share/man/man1/qtchooser.1.gz

```

