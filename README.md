# GenomicFormatExamples

This package contains small examples of various genomic file formats for demonstration purpose.

Format currently available:
* [bed](https://genome.ucsc.edu/FAQ/FAQformat.html#format1.7)
* [narrowPeak](https://genome.ucsc.edu/FAQ/FAQformat.html#format12)
* [broadPeak](https://genome.ucsc.edu/FAQ/FAQformat.html#format13)

The `demo.narrowPeak` is the first 1000 lines from the [E003-H3K27ac.narrowPeak.gz](http://egg2.wustl.edu/roadmap/data/byFileType/peaks/consolidated/narrowPeak/E003-H3K27ac.narrowPeak.gz) file[1]. The `demo.broadPeak` was generated using the first 9 columns of `demo.narrowPeak` and the `demo.bed` file using the first 6 columns.

# Installation

```
require(devtools)
install_github("charlesjb/GenomicFormatExamples")
```

# Usage

To get the path to each demo file:

```
get_demo_file(format = "bed")
get_demo_file(format = "narrowPeak")
get_demo_file(format = "broadPeak")
```

[1] Roadmap Epigenomic Consortium *et al*, 2015
