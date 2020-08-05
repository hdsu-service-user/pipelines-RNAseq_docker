FROM broadinstitute/picard

# Dockerfile modified from genomicpariscentre/samtools
RUN apt update && \
    apt install --yes wget libcurl3-gnutls && \
    wget http://mirrors.kernel.org/ubuntu/pool/universe/s/samtools/samtools_1.9-4_amd64.deb && \
    wget http://mirrors.kernel.org/ubuntu/pool/universe/h/htslib/libhts2_1.9-10_amd64.deb  && \
    dpkg -i samtools_*.deb libhts2_*.deb && \
    rm *.deb && \
    apt clean