# Libfranka Non RT Patch
Do you want to run Panda on a Non Real-Time (RT) Kernel? One of the use cases for this would be that Nvidia Drivers can be installed in an Non RT Kernel so that you can run computationally intensive tasks. One of the kernels I suggest using is [Liquorix](https://liquorix.net/#install). If that's the case then this Patch will help you.

Download your [Libfranka](https://github.com/frankaemika/libfranka) in your ROS workspace. And then download this patch named "PatchFile" from this repo and paste inside recently downloaded/cloned libfranka's root dirtectory.

Apply the patch by this command:

```bash
patch -p1 < PatchFile
```
Assuming you just downloaded this Patch File in the Libfranka directory. Now the Franka ROS server will run without any need of RT kernel. Also this will work on latest 0.8.0 and also 0.7.1 and 0.7.0. 

Disclaimer: It's always better to use RT kernel when controlling Panda. There is no substitute to that. Only use this patch if you are okay controlling Panda in a Non-Realtime fashion. 

Having to maintain a separate system for controlling Panda and having a separate system with Nvidia graphics card to maintain and run your experiements can be
a costly affair and also exhausting. I hope the main kernel supports the realtime patch into mainstream soon so that we don't have to do all of this and Nvidia supports it as well.