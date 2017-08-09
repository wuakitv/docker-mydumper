# docker-mydumper
Docker image for mydumper and myloader

Example usage:
```
docker --rm -it \
  -v $(pwd):/mydumper:rw \
  wuakitv/mydumper \
  mydumper \
    --compress \
    --build-empty-files \
    --lock-all-tables \
    --host db_hostname \
    --user username \
    --password password
```
