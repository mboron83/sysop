### Mount samba share

```
sudo mount -t cifs //192.168.1.X/myshare ~/myshare/ -o username=USERNAME,password=PASSWORD,uid=1000,gid=1000,iocharset=utf8,file_mode=0777,dir_mode=0777
```
