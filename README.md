# Libfranka Non RT Patch
Do you want to run Panda on a Non Real-Time (RT) Kernel? 

Well, this Patch will help you.

Download your [Libfranka](https://github.com/frankaemika/libfranka) in your ROS workspace. And then download this patch named "PatchFile" from this repo

Apply this patch from this repo by this command:

```bash
patch -p1 < PatchFile
```
Assuming you just downloaded this Patch File in the Libfranka directory. 

Now the Franka ROS server will run without any need of RT kernel. Congrats!!

Also this will work on latest 0.8.0 and also 0.7.1 and 0.7.0. 

If any issues raise an issue! If youu need for any previous tags, raise an Issue and be sure to tag me (@krishnachaitanya7)!