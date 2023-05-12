dozzle
---

Run Dozzle from docker image as systemd.service.

### Links:
- <https://dozzle.dev>
- <https://github.com/amir20/dozzle>
- <https://hub.docker.com/r/amir20/dozzle>


### Variables:
- **`dozzle_docker_image`** *(type=string, default="amir20/dozzle:latest")* - Docker image for run as systemd.service.
- **`dozzle_docker_network`** *(type=string, default="bridge")*
- **`dozzle_docker_publish_ports`** *(type=list, default=[])*
- **`dozzle_docker_labels`** *(type=list, default=[])*

- **`dozzle_basepath`** *(type=string, default="/")*
- **`dozzle_username`** *(type=string, default="")*
- **`dozzle_password`** *(type=string, default="")*

- **`dozzle_filter`** *(type=list, default=[])*

- **`dozzle_log_level`** *(type=string, default="error")* - Dozzle self log level: panic, fatal, error, warn, info, debug, trace.
