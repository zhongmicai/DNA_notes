# Notes on DNA sequencing-related tools and genome variation analysis

These notes are not intended to be comprehensive. They include notes about methods, packages and tools I would like to explore. For a comprehensive overview of the subject, consider [other bioinformatics resources](https://github.com/mdozmorov/blogs/tree/master/Bioinformatics). Issues with suggestions and pull requests are welcome!

# Table of content

* [Variant calling pipelines](#variant-calling-pipelines)
* [Depth](#depth)
* [InDels](#indels)
* [CNV](#cnv)
* [Functional impact](#functional-impact)
* [Misc](#misc)

## Variant calling pipelines

- TOPMed Variant Calling Pipeline, https://github.com/statgen/topmed_variant_calling

- `DNAscan` - a pipeline for DNA-seq analysis to call SNPs, indels, SVs, repeat expansions and viral genetic material. Four parts - alignment (HISAT2, BWA mem), analysis (Freebayes, GATC HC, Manta, Expansion Hunter), annotation (Annovar), report generation. https://github.com/KHP-Informatics/DNAscan
    - Iacoangeli, A., A. Al Khleifat, W. Sproviero, A. Shatunov, A. R. Jones, S. L. Morgan, A. Pittman, R. J. Dobson, S. J. Newhouse, and A. Al-Chalabi. “DNAscan: Personal Computer Compatible NGS Analysis, Annotation and Visualisation.” BMC Bioinformatics 20, no. 1 (December 2019): 213. https://doi.org/10.1186/s12859-019-2791-8.


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

- `Control-FREEC` - assess copy number and genotype information in whole genome and exome sequencing data. Corrects for contamination by normal cells and variable sample ploidy. With a matched normal sample, distinguishes somatic from germline events. http://boevalab.com/tools.html
    - Boeva, Valentina, Tatiana Popova, Kevin Bleakley, Pierre Chiche, Julie Cappo, Gudrun Schleiermacher, Isabelle Janoueix-Lerosey, Olivier Delattre, and Emmanuel Barillot. “Control-FREEC: A Tool for Assessing Copy Number and Allelic Content Using next-Generation Sequencing Data.” Bioinformatics (Oxford, England) 28, no. 3 (February 1, 2012): 423–25. https://doi.org/10.1093/bioinformatics/btr670.

- `CNVkit` - capturing CNVs in on-target and off-target genomic regions. Existing tools (CNVer, ExomeCNV, exomeCopy, CONTRA, CoNIFER, ExomeDepth, VarScan2, XHMM, ngCGH, EXCAVATOR, CANOES, PatternCNV, CODEX, Control-FREEC, cn.MOPS, cnvOffSeq, CopyWriteR). Account for GC content, mappability. Python 2.7 implementation. https://github.com/etal/cnvkit, https://github.com/etal/cnvkit-examples
    - Talevich, Eric, A. Hunter Shain, Thomas Botton, and Boris C. Bastian. “CNVkit: Genome-Wide Copy Number Detection and Visualization from Targeted DNA Sequencing.” PLOS Computational Biology 12, no. 4 (April 21, 2016): e1004873. https://doi.org/10.1371/journal.pcbi.1004873.

- `HATCHet` (Holistic Allele-specific Tumor Copy-number Heterogeneity) is an algorithm that infers allele and clone-specific CNAs and WGDs jointly across multiple tumor samples from the same patient, and that leverages the relationships between clones in these samples. https://github.com/raphael-group/hatchet
    - Zaccaria, Simone, and Benjamin J. Raphael. “Accurate Quantification of Copy-Number Aberrations and Whole-Genome Duplications in Multi-Sample Tumor Sequencing Data.” BioRxiv, January 1, 2018, 496174. https://doi.org/10.1101/496174.

- `TITAN` - a tool for predicting subclonal copy number alterations (CNA) and loss of heterozygosity (LOH) from tumour whole genome sequencing data. http://compbio.bccrc.ca/software/titan/

- `QDNASeq` - Quantitative DNA sequencing for chromosomal aberrations. https://bioconductor.org/packages/release/bioc/html/QDNAseq.html

- `SynthEx` - CNV detection from exome and whole genome sequencing.


## Functional impact

- `atSNP` - search for effects of SNPs on transcription factor binding. DB of 37 billion variant-motif pairs. Search by SNP IDs, window of SNPs, genomic location, gene, transcription factor. http://atsnp.biostat.wisc.edu/
    - Shin, Sunyoung, Rebecca Hudson, Christopher Harrison, Mark Craven, and Sündüz Keleş. “AtSNP Search: A Web Resource for Statistically Evaluating Influence of Human Genetic Variation on Transcription Factor Binding.” Edited by John Hancock. Bioinformatics, December 8, 2018. https://doi.org/10.1093/bioinformatics/bty1010.


## Misc

- DNA sequencing analysis notes from Ming Tang. https://github.com/crazyhottommy/DNA-seq-analysis

- `SNPhylo` - A pipeline to generate a phylogenetic tree from huge SNP data, https://github.com/thlee/SNPhylo, http://chibba.pgml.uga.edu/snphylo/

- Application for making ENCODE Blacklists, and links to canonical blacklists, https://github.com/Boyle-Lab/Blacklist
