FROM paterno/centos67-nu_v1_18_01-e9-prof
MAINTAINER Marc Paterno
LABEL Vendor="FNAL"
LABEL License="BSD"
RUN cd /products && \
    curl -O http://scisoft.fnal.gov/scisoft/bundles/tools/pullProducts && \
    chmod u+x pullProducts && \
    ./pullProducts $PWD slf6 uboone-04.31.00 e9 prof && \
    rm -f *.tar.bz2 *.tar.gz
COPY uboone_setup.sh /etc/uboone_setup.sh
RUN echo 'source /etc/uboone_setup.sh' >> /etc/profile

# Default command 
CMD ["/bin/bash", "-l"]
