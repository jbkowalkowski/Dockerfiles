FROM paterno/centos67-build_base_v4_9_3-e9-prof
MAINTAINER Marc Paterno paterno@fnal.gov
ENV REFRESHED_AT 2015-12-29
LABEL Vendor="FNAL"
LABEL License="BSD"
RUN cd /products \
  && curl -O http://scisoft.fnal.gov/scisoft/bundles/tools/pullProducts \
  && chmod u+x pullProducts \
  && ./pullProducts -r /products slf6 nu-v1_18_01 s26-e9 prof

COPY nu_setup.sh /etc/nu_setup.sh
RUN echo 'source /etc/nu_setup.sh' >> /etc/profile

# Default command 
CMD ["/bin/bash", "-l"]
