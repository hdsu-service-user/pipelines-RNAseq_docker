FROM broadinstitute/picard

RUN apt-get install -y build-essential

RUN wget https://github.com/samtools/samtools/releases/download/1.9/samtools-1.9.tar.bz2
RUN tar -vxjf samtools-1.9.tar.bz2
RUN cd samtools-1.9
RUN make