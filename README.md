# turnkey linux: mount windows share
what was in the TKL documentation didn't work for me, this is what I used successfully:

Find and replace:
- IP_OF_FILESERVER
- SHARE_NAME
- USERNAME (smb windows username)

```
apt-get update -y
apt-get install cifs-utils -y
mkdir /media/SHARE_NAME
mount -t cifs //IP_OF_FILESERVER/SHARE_NAME /media/SHARE_NAME -o username=USERNAME
```
