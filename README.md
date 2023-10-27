dozzle
---

Configure and run Dozzle from docker image as systemd.service.

### Links
- <https://dozzle.dev>
- <https://github.com/amir20/dozzle>
- <https://hub.docker.com/r/amir20/dozzle>


### Variables
- **`dozzle_docker_image`** *(type=string, default="amir20/dozzle:latest")* - Docker image for using into systemd.service.

- **`dozzle_docker_network`** *(type=string, default="bridge")* - Connect a container to a network as `docker run --network=...`.
- **`dozzle_docker_publish_ports`** *(type=list, default=[])* - List of strings for publish a container’s ports to the host as `docker run --publish=...`.

- **`dozzle_docker_labels`** *(type=list, default=[])* - List of objects in format `{key: value}` for set meta data on a container as `docker run --label=...`.

- **`dozzle_basepath`** *(type=string, default="/")* - Base for http router.

- **`dozzle_username`** *(type=string, default="")* - Username for authentication.
- **`dozzle_password`** *(type=string, default="")* - Password for authentication.

- **`dozzle_filter`** *(type=list, default=[])* - List with docker containers filter in [Docker `--filter` syntax](https://docs.docker.com/engine/reference/commandline/ps/#filter).

- **`dozzle_log_level`** *(type=string, default="error")* - Dozzle self log level: panic, fatal, error, warn, info, debug, trace.


### Examples
```yaml
dozzle_docker_image: amir20/dozzle:v5.1.0
dozzle_filter: [name=backend, name=frontend]
```
