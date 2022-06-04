# User Manual for using Docker for zeropdk

## Step 1

docker pull the image:

```bash
docker pull felimath/zeropdk
```

You can check the Docker Image by

```bash
docker images
```

shows:

```
REPOSITORY           TAG                 IMAGE ID            CREATED             SIZE
felimath/zeropdk           latest              ee53a51120d1        17 hours ago        1.42GB
```

## Step 2

Make sure you git pull the "demo" folder from github. Then,

```bash
cd /path_to/git_repo/demo
```

## Step 3: Run the environment

```bash

# Mac/Linux
bash start-bash-unix.sh

# Windows
cmd start-bash-windows.bat

```

This opens a bash shell within dockerdata with an isolated linux environment with pre-installed python3.7, klayout, zeropdk etc. and exposes port 42019 to your host system.

If, instead, you want to directly open jupyter notebook inside the current directory, then use the following scripts:

```bash
# Mac/Linux
bash start-jupyter-mac.sh

# Windows
cmd start-jupyter-windows.bat
```

