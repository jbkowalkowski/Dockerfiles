FROM paterno/centos67base
MAINTAINER Marc Paterno paterno@fnal.gov
ENV REFRESHED_AT 2015-12-28
LABEL Vendor="FNAL"
LABEL License="BSD"
RUN mkdir -p /products \
  && cd /products \
  && curl -O http://scisoft.fnal.gov/scisoft/bundles/tools/pullProducts \
  && chmod u+x pullProducts \
  && ./pullProducts -r $PWD slf6 build_base-v4_9_3 e9 prof

COPY build_base_setup.sh /etc/build_base_setup.sh
RUN echo 'source /etc/build_base_setup.sh' >> /etc/profile

# Default command 
CMD ["/bin/bash", "-l"]
