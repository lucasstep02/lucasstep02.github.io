# My first post! Setting up Dev Containers was fun

This is a tale of my failures and mistakes when following the *How to* guide by Brian Lovell that you can find [here](https://lovellbrian.github.io/2023/10/02/BYODImage.html). This rundown will work, just don't be like me and make assumptions, follow his directions!

## Basic setup of my failures

I want to start by saying this is no flame to anyone, especially not teaching staff! They helped heaps and assisted me as much as they could.

The fault is likely due to my own misunderstanding of instructions and errors with my existing WSL setup I've had for other courses at university.

My errors ranged from frozen VS Code applications, blank screens and non-descriptive error messages. It was not until midnight of the day the assignment was due that I finally got a working dev container and was able to attempt to get some form of working code to submit.

---

## What to avoid

- **DO NOT**, I repeat **DO NOT** try to install a WSL version of Docker CE, this will not work and will cause issues even after uninstalling all docker content from your device. I still cannot use my laptop for Docker now unless I use my Linux boot, I have broken my Windows Docker Desktop.

- If you have a WSL setup already, you will not be able to use the default *Ubuntu* version, follow the instructions and use the command `wsl --install --distribution Ubuntu-22.04` for an Ubuntu 22.04 setup. The Ubuntu default may work on initial setup, it may even say its the 22.04 LTS version but it **will not** work for dev containers, I tried.

- If your setup dev container cannot find pip and asks you to install, CHANGE YOUR KERNEL TO RECOMMENDED. The installs should all be there, especially if you are following the '00-bird-example'.

- To run the graphics driver, CUDA will ask for Visual Studio, this is **NOT** Visual Studio Code. You need the pink logo, otherwise CUDA will not download and complain at you constantly.

![](/../images/vs_vs_vsc.png "THE PINK ONE!!!")
Image [credit](https://www.tabnine.com/blog/visual-studio-vs-visual-studio-code/).
