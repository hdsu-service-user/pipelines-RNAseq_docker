FROM rocker/tidyverse

RUN apt-get update && apt-get install -y \
    libjpeg-dev \
    libbz2-dev \
    liblzma-dev

RUN R -e "BiocManager::install('GenomicRanges', update = FALSE )"
RUN R -e "BiocManager::install('Rsubread', update = FALSE )" 
RUN R -e "BiocManager::install('rtracklayer', update = FALSE )"
RUN R -e "BiocManager::install('devtools', update = FALSE )"
RUN R -e "BiocManager::install('pachterlab/sleuth', update = FALSE )"