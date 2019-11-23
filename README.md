# MicrOS-DevTools
Tools for configuring MicrOS development environment on GNU/Linux.

## Instructions:
First of all you will need to install few packages using your package manager.
You will need:
- nasm
- mtools
- curl (should be already installed, but check to be sure)
- build-essential (this varies from distribution to distribution, contains tools like make and necessary libraries)

Next up is downloading and running the `configure.sh` script supplying it with:
- `<workspace directory>` (directory where you cloned the MicrOS repo)
- `<threads count>` to use when compiling MicrOS (optional)
```
chmod +x configure.sh
./configure.sh <workspace directory> <threads count>
```
It will ask for sudo permission beacause it needs to install the cross complier to `/opt/` directory.