Part 4 -  List and Delete Container 
In this lab part, we will need a second terminal also running a shell as root.

__1.  Open a new terminal, expand it width wise (horizontally) to capture the output of the docker ps command we are going to run into it.  Also make sure it does not completely overlap the original terminal window.
We will be referring to this new terminal as T2; the original terminal will be referred to as T1.

__2.  In the new terminal (T2) become root (use the sudo -i command).
__3.  Change to the ~/Works directory:

cd /home/wasadmin/Works

__4.  Enter the following command:

docker ps

You should see an empty container table listing only the captions part of the table. 
CONTAINER ID    IMAGE   COMMAND   CREATED    STATUS     PORTS     NAMES

__5.  To see a list of all containers, whether active or inactive, run the following command: 

docker ps -a

__6.  Switch to the original terminal window (T1).                       

__7.  Enter the following command and replace the container id with the one from T2:

docker rm <container id>

Note: You may only need to type the first two or three characters of the container id and then press the Tab key - Docker will go ahead and auto-complete it.   

The container id shown to the user is, actually, the first 12 bytes of a 64 hexadecimal character long hash used by Docker to create unique ids for images and containers.

The docker ps command only shows the running containers; if you repeat the docker ps command now after you have killed the container process, it will show the empty table.

In order to view all the containers created by docker with stopped ones stashed in the history table, use the -a flag with this command.

__8.  Switch to the T2 terminal.

__9.  Enter the following command:

docker ps

Now it should show an empty table. 

