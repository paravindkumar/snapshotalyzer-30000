# snapshotalyzer-30000

Demo project to manage EC2 instance snapshots

## About

This project is a demo, and use boto3 to manage AWS EC2 instance snapshots.

## Configuring

shotty uses the configuration file created by the AWS cli. e.g.

`aws configure --profile shotty`

## Running

`pipenv run python shotty/shotty.py <command> <subcommand> <--project=PROJECT>`

*command* is instances, volumes, or snapshots
*subcommand* - depends on command
*project* is optional


reference to boto3 documentation
https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/index.html


Setup Tools for packaging and distribution
`pipenv install -d setuptools`

to create a binary distribution file
`pipenv run python setup.py bdist_wheel`

install snapshotanlyser
`pip3 install dist/snapshotalyzer_30000-0.1-py3-none-any.whl`

to verify the snapshotanlyzer is install
`pip3 show snapshotalyzer_30000`


