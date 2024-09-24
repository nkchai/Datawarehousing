# Dremio on Docker


* Install Docker Desktop from this [link](https://www.docker.com/products/docker-desktop/).
* In the terminal pull the dremio docker image.

    ```
    docker pull dremio/dremio-oss
    ```
* Deploy the docker image from the terminal.
    ```
    docker run -p 9047:9047 -p 31010:31010 -p 32010:32010 -p 45678:45678 dremio/dremio-oss
    ```
* Open `localhost:9047` in a browser to access dremio.

