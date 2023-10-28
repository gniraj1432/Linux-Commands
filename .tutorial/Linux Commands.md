# 50 Linux Commands - 5 min read

ls - list the files and directories in the current directory

```python
ls
```

cd - change the current directory

```python
cd dir_name
```

mkdir - create a new directory

```python
mkdir niraj
```

rmdir - remove a directory

```python
rmdir niraj
```

pwd - print the current working directory

```python
pwd
```

cp - copy files or directories

```python
#We will copy a file called example.txt from the current directory to a directory called backup
cp example.txt backup/
```

mv - move or rename files or directories

```python
mv example.txt backup/
```

rm - remove files or directories

```python
rm example.txt
```

touch - create a new empty file or update the timestamp of an existing file

```python
touch shayan.txt
```

cat - concatenate and display files

```python
cat example.txt
```

man - manual for a command

```python
man ls
```

htop - an interactive process viewer and system monitor

```python
htop
```

chmod - change the permissions of a file or directory

```python
# The first digit represents the owner of the file/directory
# The second digit represents the group that the file/directory belongs to
# The third digit represents all other users
# 0 (no permission)
# 1 (execute only)
# 2 (write only)
# 3 (write and execute)
# 4 (read only)
# 5 (read and execute)
# 6 (read and write)
# 7 (read, write, and execute)

chmod 700 file.txt
```

chown - change the owner of a file or directory

```python
chown new_owner example.txt
```

tar - create or extract compressed archive files

```python
# x: extract files from an archive
# t: list the contents of an archive
# r: append files to an existing archive
# z: use gzip compression
# j: use bzip2 compression
# cf: create file
#xf: extract file
tar cf archive.tar file1 file2 file3
```

gzip - compress files

```python
gzip file.txt
```

gunzip - decompress compressed files

```python
gunzip file.txt.gz
```

ssh - connect to a remote server securely

```python
ssh username@server_address
```

scp - securely copy files between systems

```python
scp myfile.txt user@remotehost:/home/user/
```

ping - test network connectivity

```python
ping 8.8.8.8
```

ifconfig - display or configure network interfaces

```python
ifconfig
```

netstat - display network connection information

```python
netstat
```

route - view or configure network routing tables

```python
route [options] [add/delete/show]
```

top - display system resource usage and processes

```python
top
```

ps - display information about running processes

```python
ps aux
```

kill - terminate a process

```python
kill [PID]
```

systemctl - control system services and settings

```python
# Start the nginx service
systemctl start nginx

# Check the status of the nginx service
systemctl status nginx

# Stop the nginx service
systemctl stop nginx
```

service - control system services

```python
service apache2 start
```

useradd - add a new user to the system

```python
useradd harry
```

passwd - change the password for a user

```python
passwd harry
```

userdel - delete a user from the system

```python
userdel harry
```

su - switch user to become another user

```python
su john
```

sudo - execute a command as another user or with elevated privileges

```python
sudo
```

uptime - display system uptime and load average

```python
uptime
```

df - display disk space usage

```python
df
```

du - display disk usage by file or directory

```python
du
```

mount - mount a file system

```python
sudo mount /dev/sdb1 /mnt/usb
```

umount - unmount a file system

```python
sudo umount /mnt/usb
```

date - display or set the system date and time

```python
date
```

whoami - display the current user name

```python
whoami
```

which - locate a program or command in the system path

```python
ls
```

finger - displays all the information about user

```python
finger harry
```

uname - display system information

```python
uname
uname -a
```

history - display a list of previously executed commands

```python
history
```

echo - display text or variables to the console

```python
echo 'I need Tshirt from codeswear!'
```

tee - redirect output to both a file and the console

```python
$ ls | tee file.txt
```

locate - locate any file on the system

```python
locate file.txt
```

sort - sort lines of text in a file or input

```python
cat file.txt
banana
orange
apple
sort file.txt
apple
banana
orange
```

uniq - remove duplicate lines from a file or input

```python
cat file.txt
apple
orange
banana
apple
banana
uniq file.txt
apple
orange
banana
```

head/tail - display the first/last few lines of a file or input

```python
#display first 10 lines
head file.txt

#display last 10 lines
tail file.txt
```