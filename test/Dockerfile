FROM dsccadminch/onyxia-rstudio:r4.5.1 

# # Temporarily switch to root user to update stuff
USER root

RUN apt-get update && apt upgrade -y
# Fix permissions so non-root users can execute pam-helper

RUN chmod +g -R /usr/lib/rstudio-server

USER 1001010000