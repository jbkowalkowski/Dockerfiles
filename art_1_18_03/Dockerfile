FROM paterno/centos67base
MAINTAINER Jim Kowalkowski
LABEL Vendor="FNAL"
LABEL License="BSD"
RUN mkdir /products
RUN cd /products && curl -O http://scisoft.fnal.gov/scisoft/bundles/tools/pullProducts && chmod u+x pullProducts && ./pullProducts $PWD slf6 art-v1_18_03 e9 prof

COPY build_base_setup.sh /etc/build_base_setup.sh
RUN echo 'source /etc/build_base_setup.sh' >> /etc/profile
# Default command 
CMD ["/bin/bash"]

