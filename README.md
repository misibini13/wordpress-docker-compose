This docker compose file, includes mounting a directory from the host to store WordPress files (like public_web). This allows persistence and easier file management.

    - ./public_web:/var/www/html: This mounts the public_web folder from your host machine into the container at /var/www/html (WordPress's default web root).

    Any changes in ./public_web on the host will reflect inside the container and vice versa.

    This setup ensures WordPress data persists even if the container is removed.
