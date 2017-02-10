## phpsepc - SpecBDD Framework for PHP
[![Docker Pulls](https://img.shields.io/docker/pulls/rvannauker/phpspec.svg)](https://hub.docker.com/r/rvannauker/phpspec/) [![Docker Stars](https://img.shields.io/docker/stars/rvannauker/phpspec.svg)](https://hub.docker.com/r/rvannauker/phpspec/) [![](https://images.microbadger.com/badges/image/rvannauker/phpspec:latest.svg)](https://microbadger.com/images/rvannauker/phpspec:latest) [![GitHub issues](https://img.shields.io/github/issues/RichVRed/docker-phpspec.svg)](https://github.com/RichVRed/docker-phpspec) [![license](https://img.shields.io/github/license/RichVRed/docker-phpspec.svg)](https://tldrlegal.com/license/mit-license)

Docker container to install and run phpspec

### Installation / Usage
1. Install the rvannauker/phpspec container:
```bash
docker pull rvannauker/phpspec
```
2. Run phpspec through the phpspec container:
```bash
sudo docker run --rm --volume $(pwd):/workspace --name="phpspec" "rvannauker/phpspec" run
```

### Download the source:
To run, test and develop the PHPSPEC Dockerfile itself, you must use the source directly:
1. Download the source:
```bash
git clone https://github.com/RichVRed/docker-phpspec.git
```
2. Build the container:
```bash
sudo docker build --force-rm --tag "rvannauker/phpspec" --file phpspec.dockerfile .
```
3. Test running the container:
```bash
 $ docker run rvannauker/phpspec --help
```