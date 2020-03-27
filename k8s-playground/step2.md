Part 3 -  Run the "Hello World!" Command on Docker 

Let's check out what OS images are currently installed on your Lab Server.

__1.  Enter the following command:

docker images

Notice there are a few images in the VM. You will use them in various labs. 

One of the images is ubuntu:12.04.

__2.  Enter the following command:

docker run ubuntu echo 'Yo Docker!'

Notice it displays Yo Docker! message

So, what happened?
docker run executes the command that follows after it on a container provisioned on-the-fly for this occasion.   

When the Docker command completes, you get back the command prompt, the container  gets stopped and Docker creates an entry for that session in the transaction history table for your reference.
