# awscli

[![Build Status](https://travis-ci.org/katosys/awscli.svg?branch=master)](https://travis-ci.org/katosys/awscli)

AWS command line interface.

#### Show the command help:
```
docker run -it --rm katosys/awscli help
```

#### Download a file to the current working directory:
```
docker run -it --rm \
--volume ${HOME}/.aws:/root/.aws \
--volume ${PWD}:/aws \
katosys/awscli:v1.10.47-1 \
s3 cp s3://my_bucket/my_file .
```
