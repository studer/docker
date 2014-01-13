# ipython notebook
#
# VERSION       1

# use the ubuntu base image provided by dotCloud
FROM studer/arch

MAINTAINER studer hello@studer.su

# install memcached
RUN pacman -S --noconfirm ipython2 python2-tornado python2-jinja python2-pyzmq

# Launch ipython2 when launching the container
ENTRYPOINT ["ipython2", "notebook"]

# run ipython2 as the daemon user
USER daemon

# expose ipython2 port
EXPOSE 8888
