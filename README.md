# sis2021_final

![alt text](figs/example.png)

-----------

**Before you clone this repo, please make sure ssh key is used for Github. If you don't use ssh key, please refer this [tutorial](tutorials/00-ssh-key.md).**
```
 $ ssh -T git@github.com
 Hi XXX! You’ve successfully authenticated, but GitHub does not provide shell access.
```

## Clone repo
```
 $ git clone --recursive git@github.com:Sensing-Intelligent-System/sis2021_final.git
```

## Update the sis2021_gazebo
```
 $ source git_pull.sh
```

### For gpu machines
```
 $ cd Docker/gpu/ && source docker_run.sh
```
or
```
 $ source gpu_run.sh
```

### For cpu machines
```
 $ cd Docker/cpu/ && source docker_run.sh
```
or
```
 $ source cpu_run.sh
```

### If you want to enter same docker images
```
 $ source docker_join.sh
```

------------

### launch locobot gazebo for different world (grasping, placing, navigation, pushing)
```
 Docker $ cd sis2021_final && source catkin_make.sh
 Docker $ source environment.sh
 Docker $ roslaunch locobot_competition locobot_sim.launch world:=grasping
```
# marslite
# marslite
