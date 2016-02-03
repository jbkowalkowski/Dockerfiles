FROM centos:6.7
MAINTAINER Jim Kowalkowski
LABEL Vendor="FNAL"
LABEL License="BSD"
RUN yum install -y gcc
RUN yum install -y redhat-lsb-core
RUN yum install -y atk-devel apr-devel asciidoc cairo-devel libconfuse-devel libcurl-devel fontconfig-devel freetype-devel glib2-devel gtk2-devel krb5-devel libICE-devel libSM-devel libX11-devel libXext-devel libXft-devel libXi-devel libXrender-devel libXt-devel libpng-devel libstdc++-devel mesa-libGL-devel mesa-libGLU-devel ncurses-devel nss-devel openssl-devel openldap-devel pango-devel qt-devel swig texinfo xmlto zlib-devel readline-devel expat-devel libXpm-devel libXmu-devel bzip2-devel texinfo tk-devel tcl-devel gcc-c++ libgcc.i686 glibc-devel.i686 libstdc++.i686
RUN yum -y install epel-release
RUN yum install -y libconfuse-devel

# Default command 
CMD ["/bin/bash", "-l"]

