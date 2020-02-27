Containers are just normal Linux Processes with additional configuration applied. 
To be example we try to launch the following Redis container
Run this command :
docker run -d --name=db redis:alpine

"-d" tanpa isian parameter,digunakan untuk menjalankan perintah sebagai daemon (background service,tanpa log di terminal)

"--name=db" untuk memberi nama container 'db' for example (biasanya digunakan untuk keperluan delete container dan lainnya)

"redis:alpine" membuat container redis for example 

The Docker container launches a process called "redis-server"
you can see with this command :
ps aux | grep redis-server

you can see identify information about the process including PID (Process ID) and PPID (Parent Process ID)
with this command :
docker top db