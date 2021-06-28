# Magikarp Ground Mission

Q --> 
Do you know how to move between directories and read files in the shell? Start the container, `ssh` to it, and then `ls` once connected to begin. Login via `ssh` as `ctf-player` with the password, `6d448c9c`

sol --> 

start instance and login to ssh --> ssh ctf-player@venus.picoctf.net -p 55667
enter the password --> 6d448c9c

ctf-player@pico-chall$ ls
1of3.flag.txt  instructions-to-2of3.txt
ctf-player@pico-chall$ cat 1of3.flag.txt 
picoCTF{xxsh_
ctf-player@pico-chall$ cat instructions-to-2of3.txt 
Next, go to the root of all things, more succinctly `/`
ctf-player@pico-chall$ cd /
ctf-player@pico-chall$ ls
2of3.flag.txt  dev   instructions-to-3of3.txt  media  proc  sbin  tmp
bin            etc   lib                       mnt    root  srv   usr
boot           home  lib64                     opt    run   sys   var
ctf-player@pico-chall$ cat 2of3.flag.txt 
0ut_0f_\/\/4t3r_
ctf-player@pico-chall$ cat instructions-to-3of3.txt 
Lastly, ctf-player, go home... more succinctly `~`
ctf-player@pico-chall$ cd home
ctf-player@pico-chall$ ls
ctf-player
ctf-player@pico-chall$ ls -al
total 16
drwxr-xr-x 1 root       root       4096 Mar 16 06:12 .
drwxr-xr-x 1 root       root       4096 Jun 28 13:17 ..
drwxr-xr-x 1 ctf-player ctf-player 4096 Jun 28 13:18 ctf-player
ctf-player@pico-chall$ ls -a
.  ..  ctf-player
ctf-player@pico-chall$ cd ctf-player/
ctf-player@pico-chall$ ls
3of3.flag.txt  drop-in
ctf-player@pico-chall$ cat 3of3.flag.txt 
5190b070}
ctf-player@pico-chall$ Connection to venus.picoctf.net closed by remote host.
Connection to venus.picoctf.net closed.
