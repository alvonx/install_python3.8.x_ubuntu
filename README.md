# Installing python 3.8.x in ubuntu

## Step 1 
- `sudo apt update`

## Step 2
- `sudo apt install build-essential zlib1g-dev libncurses5-dev libgdbm-dev libnss3-dev libssl-dev libreadline-dev libffi-dev libsqlite3-dev wget libbz2-dev
`

## Step 3 (replace x with the version you want to install e.g. x=5,10)
export PYTHON38_VERSION=<x>

## Step 4 
- `wget https://www.python.org/ftp/python/3.8.$PYTHON38_VERSION/Python-3.8.$PYTHON38_VERSION.tgz`

## Step 5
- `tar -xf Python-3.8.$PYTHON38_VERSION.tgz`

## Step 6
- `cd Python-3.8.$PYTHON38_VERSION`

## Step 7
- `./configure --enable-optimizations`

## Step 8 (value after j represent number of cores)
- `make -j 8`

## Step 9
- `sudo make altinstall`

## Step 10 (verify installed version of python3.8)
- `python3.8 --version`
