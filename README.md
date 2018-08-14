# Purpose

This image is the base image for all my other images.  It's a basic Debian Stretch (based on the official slim version found on hub.docker.com) with configuration done to Asynchrone's needs.

## Configuration changes

- The timezone is set to "Europe/Brussels" by default, but it can be overriden as it is a configuration argument.
- apt-utils is installed: apt-get otherwise gives a warning about it.
- /root/.bashrc file for colorized ls command

# Open Source

The reason to open source the code of this image, together with the Gradle project, is only because other images that have a more specific purpose are built upon this image.
It might not be such a good idea to base your own images upon this image.

# Support

This image is supported and maintained by Asynchrone. If you have any problems, bugs or questions, please contact info@asynchrone.com. Asynchrone will provide the best support possible. However, as this is a free and open source image, Asynchrone cannot guarantee any timing, nor solution. If you want a higher level of support, you may want to consider a paid support option. Contact yves.vindevogel@asynchrone.com for paid support questions.

# TODO

- Update the sources.list.d with a file specific to OVH. Before I put a file, I want to see how OVH configures their Debian servers.
