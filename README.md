# sysadmiral-docker-dockerfiles

## per dockerfile instructions

- [python3](#python3)
  - [Description](#description)
  - [Usage](#usage)
- [saws](#saws)
  - [Description](#description)
  - [Usage](#usage)

### python3

#### Description

This is a small container based on `alpine:latest` that installs `python3` from 
the official apk repositories.

It then install `pip` and `setupttools` and updates them to the latest version.

#### Usage

```shell
docker pull sysadmiral/python3
```

### saws

#### Description

This container runs `SAWS` - A supercharged AWS command line interface (CLI).

Information about `SAWS` is available here: <https://github.com/donnemartin/saws>

To use this container you will need to set up a folder for storing your
AWS credentials. If you use multiple profiles you will need to have a folder per
profile.

When you `docker run` you can then mount that credentials dir and `SAWS` will
log you into the correct account.

#### Usage

```shell
docker pull sysadmiral/saws
docker run -it -v $YOUR_CREDS_FILE_DIR:/root/.aws:ro sysadmiral/saws
```
