# Hub Image Template
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/nmfs-opensci/cefi-image/HEAD)
[![Build and push container image](https://github.com/nmfs-opensci/cefi-image/actions/workflows/repo2docker.yaml/badge.svg)](https://github.com/nmfs-opensci/cefi-image/actions/workflows/repo2docker.yaml)

A repository for creating an environment image for a Jupyter Hub. The main purpose is to help users create custom images for JupyterHubs, expecially if they need to add command line tools to the image.  

## How to use? 

* Add packages: Edit `binder/environment.yml`. The new image will automatically build.
* Add system libraries: Add `binder/apt.txt`. No comments. One package per line.

## How to test

Go to [mybinder.org](https://mybinder.org/). Copy the url for the repo into the box. Or you can click the 'Open in Binder' badge above.

## Using this in JupyterHub

The image will appear under packages in the right nav area of your GitHub repo. If the JupyterHub has the **Bring your own image** feature, then you can paste in `ghcr.io/nmfs-opensci/cefi-image:latest`.

<img width="772" alt="image" src="https://github.com/user-attachments/assets/13f1d200-b8a6-44e1-a9db-537260b21ec4">

