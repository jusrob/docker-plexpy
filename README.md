Docker container for the python program plexpy used to monitor and analyze your Plex server usage.

The plexpy database and logs are stored in the /data volume. I mount that volume to my docker host. To start use the following command:

```docker run --name="plexpy" --publish=8181:8181 --volume=/data/warehouse/plexpy:/data --restart="always" --detach=true jusrob/plexpy```
