Containers Tutorial
===================

Docker is a platform for developing, shipping, and running applications inside containers. Containers are lightweight, portable, and ensure that applications run consistently across different environments.

What is a Docker Image?
-----------------------
A Docker image is a pre-configured package that contains everything needed to run an application, including the code, runtime, libraries, and dependencies. Once an image is instantiated, it becomes a container, which is an isolated runtime environment.

Prerequisites
-------------
Before you begin, ensure that you have the following:
    - A system with NVIDIA GPU for CUDA support (which TACC machines do)
    - A working internet connection to download Docker.

Steps to Install PyTorch with CUDA on Docker
--------------------------------------------
**Step 1: Install Docker (if not already installed)**

    - `Mac <https://docs.docker.com/desktop/setup/install/mac-install/>`_
    - `Windows <https://docs.docker.com/desktop/setup/install/windows-install/>`_
    - `Linux <https://docs.docker.com/desktop/setup/install/linux/>`_

**Step 2: Open up the Docker Command Line Interface**

Ensure that Docker is running, then open the integrated terminal.

**Step 3. Pull a Prebuilt PyTorch Doocker Image**

Instead of creating our own Dockerfile, we can use an official PyTorch image from DockerHub

.. note::

    DockerHub is official cloud-based repository where developers store, share, and distribute Docker images. Similar to GitHub but for Docker containers.

Run the following command to pull the latest PyTorch image with CUDA support.

::
    
    docker pull pytorch/pytorch:2.5.1-cuda12.4-cudnn9-devel

CUDA is an API that allows software to utilize NVIDIA GPUs for accelerated computing. This is essential for deep learning because GPUs process tasks much faster than CPUs.
Since TACC machines have NVIDIA GPUs, we must use a CUDA-enabled PyTorch image to fully leverage GPU acceleration.



**Step 4. Run a Container**

Once the image is downloaded, we can create and run a Docker container from it:

:: 

    docker run --gpus all -it --rm pytorch/pytorch:2.5.1-cuda12.4-cudnn9-devel

Flags: 
-it -> interactive terminal
-- rm -> removes the container after exit.
--gpus all -> enable GPU access for CUDA-enabled containers

**Step 5. Run a PyTorych Script Inside the Container**

    Once inside the container, start Python

::

    python

