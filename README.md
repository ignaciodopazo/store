# store
Points to repositories with frontend and backend respectively of an e-store (i.e. have them as submodules): custom versions of commerce as FE and vendure as BE.

## Development notes

### Working with submodules
After cloning this repo, you should initialize and update the submodules
```
git submodule init
git submodule update
```
which ends up cloning the submodules in your local.


To keep your local submodules up to date you can run at the store repo
```
git pull --recurse-submodules
```
For more info about git submodules check https://gist.github.com/gitaarik/8735255.

### Utility bash script for develop

#### Steps to start you environment in a gnome terminal (e.g. Ubuntu 20.04)
1. Create a file named `store.env.sh` with content taken from `store.env.sh.template`
2. Declare the env variable `STORE_ROOT` as the path of this repository in your local machine
3. Finally, run the `store.env.sh` script with the following command
```
. store-env
```
or
```
source store-env
```

