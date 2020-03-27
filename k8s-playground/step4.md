Part 5 -  Working with Containers

__1.  Switch to the T1 terminal.

__2.  Enter the following command:

docker run -it --hostname basic_host ubuntu /bin/bash

This command will create a container from the ubuntu OS image, it will give the instance of the container the hostname of basic_host, launch the bash program on it and will make the container instance available for interactive mode (i) over allocated pseudo TTY (t). 

After running the above command, you should be dropped at the prompt of the basic_host container.

	root@basic_host:/#
As you can see, you are root there (symbolized by the '#' prompt sign).

__3.  Enter the following command to stop the container and exit out to the host OS:

	exit 

	You should be placed back in the root's Works folder.

__4.  Enter the following command to see the containers:

	docker ps -a
	You should see the status as Exited.
__5.  Enter the following command to restart the container (pick the new one from the list):
	docker start <container id>
__6.  Connect to the container:
	docker exec -it <container id> /bin/bash
__7.  Enter the following command:
	exit
	You should be logged off and placed back in the root's Works folder.
__8.  Enter the following command:
	docker stop <container id>
__9.  Enter the following command:

	docker ps -a
	You should see that the container is listed in the transaction history. 
	CONTAINER ID        IMAGE               COMMAND             CREATED             STATUS                     PORTS                    NAMES
	aed47e954acd        ubuntu              "/bin/bash"         3 minutes ago      Exited (0) 4 minutes ago        amazing_panini   
	...
