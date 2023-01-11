# jupyter
A collection of jupyter notebooks I use to work with my data.<br>
To run Jupyter on Docker:<br>
Install Docker for your platform, this should be easy to find.<br>
Makes it easier to set things up to run non-root:<br>
https://docs.docker.com/engine/install/linux-postinstall/#manage-docker-as-a-non-root-user<br>
TL;DR<br>
`sudo groupadd docker` # might respond with: groupadd: group 'docker' already exists<br>
`sudo usermod -aG docker yourusername`<br>
Log out and log back in<br>
`docker run hello-world` # test without sudo<br>

Run command below in the dir that contains the notebooks<br>
`docker run -p 8888:8888 -v $(pwd):/home/jovyan/work jupyter/scipy-notebook`<br>
Follow instructions to access Jupyter<br>
Double click on work dir to see files from pwd<br>
Short version of instructions found at:<br>
https://towardsdatascience.com/how-to-run-jupyter-notebook-on-docker-7c9748ed209f<br>
