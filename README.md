# Notes on DNA sequencing-related tools and genome variation analysis

These notes are not intended to be comprehensive. They include notes about methods, packages and tools I would like to explore. For a comprehensive overview of the subject, consider [other bioinformatics resources](https://github.com/mdozmorov/blogs/tree/master/Bioinformatics). Issues with suggestions and pull requests are welcome!

# Table of content

* [Depth](#depth)
* [InDels](#indels)
* [CNV](#cnv)


## Depth

- `mosdepth` - fast BAM/CRAM depth calculation for WGS, exome, or targetted sequencing., https://github.com/brentp/mosdepth
- `indexcov` - fast genome coverage, aberrant coverage detection, infer sex. Visualization. https://github.com/brentp/goleft
- `bamCoverage` - BAM to bigWig conversion, https://deeptools.readthedocs.io/en/latest/content/tools/bamCoverage.html


## InDels

- `Pindel` - breakpoints of large deletions, medium sized insertions, inversions, tandem duplications and other structural variants. http://gmt.genome.wustl.edu/packages/pindel/

- `Dindel` - Accurate indel calls from short-read data. http://www.sanger.ac.uk/science/tools/dindel

- `Destruct` - joint prediction of rearrangement breakpoints from single or multiple tumour samples. https://bitbucket.org/dranew/destruct.git

- `MindTheGap` - detection and assembly of DNA insertion variants, https://gatb.inria.fr/software/mind-the-gap/, https://github.com/GATB/MindTheGap

- `Breakfast` - a software for detecting genomic structural variants from DNA sequencing data, https://github.com/annalam/breakfast


## CNV

- `TITAN` - a tool for predicting subclonal copy number alterations (CNA) and loss of heterozygosity (LOH) from tumour whole genome sequencing data. http://compbio.bccrc.ca/software/titan/

- `QDNASeq` - Quantitative DNA sequencing for chromosomal aberrations. https://bioconductor.org/packages/release/bioc/html/QDNAseq.html

- `SynthEx` - CNV detection from exome and whole genome sequencing.
