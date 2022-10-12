# gp6
This week’s assignment is to “containerize” your Python app so that it can be distributed and run using Docker. Your goal is to end up with a Docker container imageLinks to an external site. that is uploaded to the Docker public repository hub.docker.comLinks to an external site.. Your guide for this project are the instructions found in steps 1–2 of the Docker Tutorial module in Canvas. You will also want to have completed the Learning DockerLinks to an external site. lab assignment before you do this, because it will introduce you to fundamental concepts of containers and VMs.

I will be automating the grading of this assignment using a script that will pull the Docker image using the URL you submit in Canvas, launch the container, then test the JSON output for an expected result (using the same test suite that I already showed you for project #5). I will be launching the container with this command:

$ docker run -p 8000:4000 <container_name>
This means that your container should be using port 4000 to serve its API. You should submit your Docker Hub URL to Canvas; it should be of the form:

https://hub.docker.com/r/<docker_username>/<image>
The grading criteria for this project will be whether I can successfully pull the container and launch it, and the percentage of tests that it passes (which means that if you haven’t already corrected any outstanding error from project #5, you must do so!).
