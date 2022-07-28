# Simple FTP Server

## About The Project
An small x86-32/x64 FTP Server.

## Support FTP Server Command
- USER
- PASS
- PASV
- LIST
- CWD
- PWD
- MKD
- RMD
- RETR
- STOR
- DELE
- SIZE
- ABOR
- QUIT
- TYPE
- NOOP
- NLST

## Compile
```
[Ftp directory]$ make
```
## Usage
### Server Side
Just run the execute file.
```
[Ftp directory]$ ./SimpleFtpServer
```
### Client Side
- Connect to server
```
[Any directory]$ ftp <Server-IP> 8021
```
- Username list for anonymous ftp (No password required)
  - ftp
  - anonymous
  - test
 - In order to use all FTP commands properly, remember to enter passive mode first. 
   -   `ftp> passive`
## Changelog

### 2022/07/28
Release 1st version. 

#### New features:
- Support the basic FTP client `mget` command

#### New rules:
- Add NLST command function
- Add wildcard related functions
  - `ISWildCard` function
  - `FileNameMapping` function    


## Reference
This program is a modification of [Siim](https://github.com/Siim/ftp) 's work.

