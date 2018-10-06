Table of Contents
=================

  * [Table of Contents](#table-of-contents)
    * [Ready to use containers](#ready-to-use-containers)
    * [Projects](#projects)
      * [hashicorp\-vault](#hashicorp-vault)
      * [test\-kitchen](#test-kitchen)
      * [curl\-loader](#curl-loader)
      * [etsy\-mixer](#etsy-mixer)
      * [CentOS x86\_64](#centos-x86_64)
    * [Manual build example](#manual-build-example)
  * [Useful bash aliases](#useful-bash-aliases)
  * [Credits](#credits)

## Ready to use containers
You can find fully baked containers, using the [dockerfiles](https://github.com/kintoandar/dockerfiles) provided in this repository, on the public [docker registry](https://hub.docker.com/u/kintoandar/)

## Projects
These are the currently available projects

------

### hashicorp-vault
[![Docker Pulls](https://img.shields.io/docker/pulls/kintoandar/hashicorp-vault.svg?maxAge=3600)](https://hub.docker.com/r/kintoandar/hashicorp-vault/)

[Hashicorp Vault](https://blog.kintoandar.com/2015/11/vault-PKI-made-easy.html) on a tiny busybox

```
# Run example

docker run -p 8300:8300 kintoandar/hashicorp-vault
```

------

### test-kitchen
[![Docker Pulls](https://img.shields.io/docker/pulls/kintoandar/test-kitchen.svg?maxAge=3600)](https://hub.docker.com/r/kintoandar/test-kitchen/)

Fully provisioned [CentOS x86_64](https://blog.kintoandar.com/2014/11/cooking-with-containers.html)  container with  [test-kitchen](https://blog.kintoandar.com/2014/11/cooking-with-containers.html) to enable easy chef cookbook testing

------

### curl-loader
[![Docker Pulls](https://img.shields.io/docker/pulls/kintoandar/curl-loader.svg?maxAge=3600)](https://hub.docker.com/r/kintoandar/curl-loader/)

Installs [curl-loader](https://github.com/kintoandar/dockerfiles/tree/master/curl-loader) on a clean CentOS x86_64

------

### etsy-mixer
[![Docker Pulls](https://img.shields.io/docker/pulls/kintoandar/etsy-mixer.svg?maxAge=3600)](https://hub.docker.com/r/kintoandar/etsy-mixer/)

Installs [etsy mixer platform](https://codeascraft.com/2015/09/15/assisted-serendipity/) for testing

------

### CentOS x86_64
[![Docker Pulls](https://img.shields.io/docker/pulls/kintoandar/centos-6.5-x86_64.svg?maxAge=3600)](https://hub.docker.com/r/kintoandar/centos-6.5-x86_64/)

This container was built from scratch to have the smallest size footprint and it's currently being used by some of my dockerfiles

You may have a look in my [kickstart files](https://github.com/kintoandar/rtfm/tree/master/kickstart)

------

## Manual build example
If you want to build the container yourself, here's an easy to follow example:

``` shell
git clone https://github.com/kintoandar/dockerfiles.git
cd dockerfiles/curl-loader
docker build .
```


# Useful bash aliases
You can find some useful bash aliases for interacting with the docker server on my [dotfiles repo](https://github.com/kintoandar/dotfiles/blob/master/.bashrc.d/docker)

# Credits
Made with ♥️ by [kintoandar](https://blog.kintoandar.com)
