# docker-and-git

* To build a docker image `git:latest` with `git` executable inside using `Dockerfile` from this repo: `docker build -t git:latest .`
* Clone this repo using `git:latest` image inside inside some folder (here`/tmp/repo`): `docker run --rm --volume /tmp/repo:/repo --workdir /repo git clone https://github.com/tejksat/docker-and-git.git .`
* Test the repo cloned: `docker run --rm --volume /tmp/repo:/repo --workdir /repo git log`
