Bootstrap: docker
From: fedora

%environment
    PATH=/opt/anaconda-ete3/bin:$PATH
    export PATH

%post
    dnf -y update && 
    dnf -y install python python-devel PyQt4 numpy python-lxml python-six python-pip gcc gcc-c++ redhat-rpm-config wget bzip2 findutils which
    wget https://repo.continuum.io/miniconda/Miniconda2-latest-Linux-x86_64.sh
    bash Miniconda2-latest-Linux-x86_64.sh -b -p /opt/anaconda-ete3
    export PATH=/opt/anaconda-ete3/bin:$PATH
    conda install -y -c etetoolkit ete3 ete_toolchain ete3_external_apps
    unlink /opt/anaconda-ete3/lib/libstdc++.so.6
    ln -s /opt/anaconda-ete3/lib/libstdc++.so.6.0.24 /opt/anaconda-ete3/lib/libstdc++.so.6

%runscript
    ete3 "$@"
