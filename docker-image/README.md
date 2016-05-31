This directory contains the files necessary to run a Docker container
with Zeppelin pre-installed and the data used in the accompanying notebook.
The steps to run the Zeppelin notebook are as follows:

1. Start the *Docker Quick Start Terminal*.
2. In the *Docker Quick Start Terminal* use `cd` to change to `<working-directory>/datenanalyse-mit-spark/docker-image`
(here `<working-directory>` is the directory containing the clone of this repository).
3. Run `docker build -t codecentric/zeppelin .` (this will take some time) 
and then `docker run --net=host -p 8080:8080 -it codecentric/zeppelin`. The `--net` flag
is used to allow internet access via the host. This is used in the notebook to download
the Databrick CSV parsing dependency.
4. Open [Link](http://192.168.99.100:8080/#/) in your browser to open the Zeppelin UI.
5. In the Zeppelin UI use **Import Notebook** to upload the notebook from `<working-directory>/million-songs/docker-image/notebooks`.

To stop the container open a second Quick Start Terminal (the one open already contains logs from Zeppelin) and use `docker ps` to obtain the container id
and then `docker stop <the container id>` to stop the container. Before this you might want to commit changes to the container, e.g. the uploaded
notebook and changes you made to it. For this first use `docker ps` to find the id of the container and then `docker commit <the container id> codecentric/zeppelin`
to commit those changes. After this you can stop the container as described with all your changes saved and available when you run
the container (as described above) the next time.