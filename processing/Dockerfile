FROM broadinstitute/picard

# Dockerfile modified from genomicpariscentre/samtools
RUN apt-get update && \
    apt install --yes wget libcurl3-gnutls && \
    wget http://ftp.br.debian.org/debian/pool/main/g/glibc/libc6_2.31-3_amd64.deb && \
    wget http://mirrors.kernel.org/ubuntu/pool/universe/s/samtools/samtools_1.9-4_amd64.deb && \
    wget http://mirrors.edge.kernel.org/ubuntu/pool/universe/libd/libdeflate/libdeflate0_1.6-1_amd64.deb && \
    wget http://mirrors.kernel.org/ubuntu/pool/universe/h/htslib/libhts2_1.9-10_amd64.deb  && \
    dpkg -i libc6_*.deb samtools_*.deb libdeflate0_*.deb libhts2_*.deb && \
    rm *.deb && \
    apt clean