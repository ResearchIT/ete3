Bootstrap: docker
From: fedora

%environment
    PATH=/opt/miniconda/bin:$PATH
    export PATH
    export LD_LIBRARY_PATH
    source /opt/miniconda/bin/activate

%post
    dnf -y update && dnf -y install python python-devel PyQt4 numpy python-lxml python-six python-pip gcc gcc-c++ redhat-rpm-config wget bzip2 findutils which
    wget https://repo.continuum.io/miniconda/Miniconda2-latest-Linux-x86_64.sh
    bash Miniconda2-latest-Linux-x86_64.sh -b -p /opt/anaconda-ete3
    export PATH=/opt/anaconda-ete3:$PATH
    conda install -y -c etetoolkit ete3 etetoolchain ete3_external_apps

%runscript
    ete3 "$@"
