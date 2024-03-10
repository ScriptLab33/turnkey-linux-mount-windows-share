# turnkey linux: mount windows share
what was in the TKL documentation didn't work for me, this is what I used successfully:

mount -t cifs //IP_OF_FILESERVER/SHARENAME /media/shared -o username=USERNAME
