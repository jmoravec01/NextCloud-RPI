# NEXTCLOUD SERVICE ON RASPBERRY PI

**OS:** Raspberry Pi OS Lite 64-bit (Debian)

**RPI version:** Raspberry Pi 5 - 8GB version

## DESCRIPTION

Running application called [NextCloud](https://nextcloud.com/) locally, works fine as NAS.

There is a possibiltiy to open NextCloud to the internet but there are another requirements - **public IP** or use of **tunneling** (for example [Ngrok](https://ngrok.com/)). This won´t be discussed in this project as it has some security reasons for me to make it public.

_Remember that opening your local network to the internet is a risk!_

**Why NextCloud?**

1. **Store your data privately**: Like a personal Dropbox or Google Drive, but you control where it's stored (on your own server or cloud storage).

2. **Access your data from anywhere**: Web interface, mobile apps, and desktop sync keep your files accessible.

3. **Collaborate with others**: Share files and folders securely with colleagues or friends.

4. **Use various apps**: Extend functionality with calendars, contacts, notes, and other productivity tools.

## REQUIREMENTS

- Docker Engine

  You can test this via `docker ps`

- Docker Compose

## HOW TO RUN

1. create folder (for example "LTP_ukol")
2. open terminal in this folder (right click for Windows - open in terminal)
3. `git clone https://github.com/jmoravec01/NextCloud-RPI.git`
4. `cd NextCloud-RPI/`
5. setup [.env](env_file.md) file
6. `docker compose up -d`
7. **done**, just connect and register in the NextCloud app

## HOW TO CONNECT

Go to the web browser and type `https://localhost:80/` (if you are hosting it on your own pc) or `https://ip_of_your_server:80/`
