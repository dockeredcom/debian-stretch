# Purpose

This image is the base image for all other dockeredcom images.  It's a basic Debian Stretch (based on the official slim version found on hub.docker.com) with some extra configuration done.

## Configuration changes

- The timezone is set to "Europe/Brussels" by default, but it can be overriden as it is a configuration argument. (Asynchrone is a Belgian company and is the owner of dockered.com)
- apt-utils is installed: apt-get otherwise gives a warning about it.
- /root/.bashrc file for colorized ls command.

# Open Source

The reason to open source the code of this image, together with the Gradle project (on GitHub), is only because other images that have a more specific purpose are built upon this image.

**It might not be such a good idea to base your own images upon this image.**

# Support

This image is supported and maintained by Asynchrone.  Asynchrone is the owner of dockered.com (and user dockeredcom). If you have any problems, bugs or questions, please contact info@dockered.com or info@asynchrone.com. Asynchrone will provide the best support possible. However, as this is a free and open source image, Asynchrone cannot guarantee any timing, nor solution. If you want a higher level of support, you may want to consider a paid support option. Contact yves.vindevogel@asynchrone.com for paid support questions.
