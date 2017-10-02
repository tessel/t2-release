 [![Build Status](https://travis-ci.org/tessel/t2-release.svg?branch=master)](https://travis-ci.org/tessel/t2-release)
 [![Code of conduct](https://camo.githubusercontent.com/ee50e87026b615a0348ce5f77bd088e3ea160b3d/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f2545322539442541342d636f64652532306f66253230636f6e647563742d626c75652e7376673f7374796c653d666c6174)](https://github.com/tessel/project/blob/master/CONDUCT.md)

## What is this?
This is a script to deploy new builds to AWS. Currently, it will only work for those with Tessel GCloud and AWS access (which is pretty much just @johnnyman727).

## Install

```
git clone git@github.com:tessel/t2-release.git;
cd t2-release;
npm install -g;
```
You will then need to create a `config.json` file that matches `example-config.json` but with real AWS credentials and your own compute machine details.

## Usage
```
t2-release # Releases a new build with a pacth increment from the last published version

t2-release --semver minor # Specify the semver increment ('patch', 'minor', 'major', etc.) and release
```
