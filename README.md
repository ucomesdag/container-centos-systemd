CentOS Stream Systemd Container Image
=====================

This Containerfile can build containers capable to use systemd.

[![centos build status](https://quay.io/repository/ucomesdag/centos/status "Container Repository on Quay")](https://quay.io/repository/ucomesdag/centos)

Branches
--------

This repository has multiple branches that relate to CentOS Stream versions.

|Branch  |CentOS Stream Version|Container image tag|
|--------|---------------------|-------------------|
|stream8 |8                    |stream8            |
|main    |latest (9)           |latest             |

Pull strategy
-------------

The different branches are **not** merged, they live as individual branches.

Manually starting
-----------------

```
podman run \
  --tty \
  --privileged \
  --volume /sys/fs/cgroup:/sys/fs/cgroup:ro \
  quay.io/ucomesdag/centos:stream8
```
