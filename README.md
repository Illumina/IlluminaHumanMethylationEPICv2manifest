# IlluminaHumanMethylationEPICv2manifest

## Install from GitHub or from .tar.gz

```
library(devtools)
install_github('https://github.com/Illumina/IlluminaHumanMethylationEPICv2manifest')
install.packages('IlluminaHumanMethylationEPICv2manifest_0.1.0.tar.gz',repos=NULL,type='source')
```

## Run

```
#read intensities
epicv2_example = read.metharray.exp(base='EPICv2_IDATs')

#assign annotation
annotation(epicv2_example)["array"] = "IlluminaHumanMethylationEPICv2"
annotation(epicv2_example)["annotation"] = "20a1.hg38"

#read beta into matrix
betas_epicv2_example= as.data.frame(getBeta(epicv2_example))
```
