# Setup log

Machine: Windows 11 desktop, WSL2 with Ubuntu 26.04
Started: 10 September 2026

## Installed WSL

Ran in PowerShell as administrator:
```
wsl --install
```
Restarted. 
Created Linux user account.

## Installed the toolchain

```
sudo apt update
sudo apt install build-essential cmake git python3 python3-pip python3-venv python3-dev
```

## Verified it works

Compiled and ran a hello-world:
```
g++ hello.cpp -o hello
./hello
```
Output: `C++ Works`

Python 3.14.4 imported fine.

## Problems hit

- Forgot `./` when running the compiled program, got "command not found".
  The `./` means "in this folder" and is required.