# Shelly Shell - Golang

This repository contains a basic reverse shell written in golang.

The project is a slightly modified version of the initial hershell golang reverse shell, needs additional work to bypass other AV vendors.
`https://sysdream.com/news/lab/2018-01-15-en-golang-for-pentests-hershell/`

### Build
```
make GOOS=windows GOARCH=amd64 LHOST=127.0.0.1 LPORT=9999
```
### Todo
* Add in hershell functionality while keeping it AV clean
* Check what windows syscall occurs upon command execution (and see if we can substitute it with a different one to avoid AV)
