## Gogs Docker Image

    docker run --restart always -d \
               --name=gogs \
               -v $PWD/data:/data \
               -p 10022:22 \
               -p 3000:3000 \
               aibar/gogs:0.8.43

## For SQLite use this path

    /data/gogs/data/gogs.db

## For git repositories use this path

    /data/git/gogs-repositories