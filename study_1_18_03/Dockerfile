FROM centos67-art_1_18_03_e9-prof
MAINTAINER jbk
LABEL Vendor="FNAL"
LABEL License="BSD"
# COPY myuname.sh /bin/uname
# COPY "./docker_study" /study
ADD AnalysisWork/docker_study /study
# ADD "./docker_study" /study
# ADD "/home/jbk/docker/AnalysisWork/docker_study" "/study"
RUN echo 'cd /study; source setup.sh' >> /etc/profile

# Default command 
CMD ["/bin/bash", "-l"]
