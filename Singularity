Bootstrap: docker
From: ubuntu:bionic

%labels
Author "Randall Cab White - rcwhite@stanford.edu"


##########
#%setup
##########

#Downlaod packages
%post
  apt-get -ym update
    ln -fs /usr/share/zoneinfo/America/Los_Angeles /etc/localtime
    apt-get install -y tzdata
    dpkg-reconfigure --frontend noninteractive tzdata

  apt-get -ymq install wget curl gcc gfortran python python3 python3-pip tar bzip2 make cmake build-essential \
  libturbojpeg libsdl2-dev libpoppler-cil poppler-utils libgraphviz-dev graphviz-dev graphviz gsfonts cairo-5c libcairo-5c0 \
  libcairo2 libcairo2-dev libpng-dev libpng*-dev libturbojpeg0-dev libpango1.0-dev libpangocairo-1.0-0 ghostscript \
   librsvg2-2 librsvg2-common librsvg2-dev freeglut3-dev fontconfig libfontconfig1-dev

######

%environment
  export IMAGE_NAME="graphviz_container"
%runscript
