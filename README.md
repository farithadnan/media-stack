<h1 align="center">
  <b>Media Stack</b>
  <br>
</h1>

<p align="center">
<b>Media-Stack</b> is a containerized solution designed for streamlined media management, allowing for automated downloading, organizing, and even subtitling of your favorite movies and TV shows.
</p>

## ⭐ Services

The Media-Stack services include:

- Gluetun (Surfshark)
- qBittorrent
- Radarr and Sonarr
- Prowlarr
- Bazarr
- Readarr
- FlareSolverr
- Jellyseerr
- Emby
- Nginx Proxy Manager
- MariaDb
- Adminer

## 🌵 Install

Git clone the repository:

```sh
    git clone https://github.com/farithadnan/media-stack.git
```

Edit the `.env` file and change the related settings:

- `SS_USER`: Your surfshark's credentials username.
- `SS_PASS`: Your surfshark's credentials password.
- `SS_REGION`: Your surfshark's region.
- `TZ`: Timezone that you want container to use.
- `PUID`: Unix user ID of the system user the containers will run as.
- `PGID`: Unix group ID of the system user the containers will run as.
- `QBT_WEBUI_PORT`: The port for the qBittorrent's WebUI/client.
- `NETWORK_SUBNET`: The local IP address of the machine, with a zero at the end.
- `BASE_DIR`: Your media directory.
- `DB_MYSQL_HOST`: MYSQL host name.
- `DB_ROOT_PWD`: MYSQL root password.
- `DB_USERNAME`: DB user's name.
- `DB_NAME`: DB's name.
- `DB_MYSQL_PWD`: DB's password.


## 🏃🏻‍♂️Running

In the directory where is your project is located:

```sh
    docker-compose up -d
```

You can then check the status of the container:

```sh
    docker-compose ps
```

## 🚫 Stopping

To stop the container:

```sh
    docker-compose down
```

## ⚙️ Configuring

All configuration files is inside the `./config` directory.
