#Load base image continuumio/miniconda3:24.3.0-0
FROM continuumio/miniconda3:24.3.0-0

#Load packages.
RUN conda install -c bioconda -c conda-forge bedops=2.4.41 bx-python=0.11.0 \
    homer=4.11 networkx=3.3 numpy=1.26.4 pandas=2.2.2 python=3.10.14 \
    samtools=1.20 --yes

#Delete the tarballs.
RUN conda clean --all --yes