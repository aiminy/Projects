# Projects

In sccc/bcc, my projects includes two parts:

## Statistics and bioinformatics methodology research 
The first part is about independent statistics and bioinformatics methodology research related to processing and analyzing deep sequencing data. This research has let me publish a biocoductor package:

https://bioconductor.org/packages/devel/bioc/html/PathwaySplice.html

I have submitted the paper of this biocoductor package as a leading author, and this paper is under review.

## Supply statistics and bioinformatics service
The second part is about supply statistics and bioinformatics service to cancer investigators in SCCC. This part has let me develop quite a lot of useful pipelines to help cancer biologists to enhance their understanding on cancer genomics. These pipelines include:

1.	ChipSeq: a pipeline for processing and analyzing ChipSeq data.  ChipSeq pipeline includes multiple steps. These steps include talking with cancer biologists to understand their research goal, setting up suitable design of experiment to make data analysis to be easier, getting sequencing read files(FASTQ files), quality control of FASTQ file, developing parser for dealing with sample information, alignment, quality control before peaking calling, peak calling, assessing the reproducibility of biological replicates using IDR, checking peak overlapping and binding affinity analysis, peak annotation, identifying the links with other binding profiles and motif finding. I use the following workflow to illustrate all these procedures in this pipeline.

![Image of ChipSeq](/ChipSeq.png)

2.	Pipeline for protein structure prediction
We developed this pipeline to use primary sequence data of proteins to predict protein tertiary structure, and to identify the effects of certain amino acid mutation on protein tertiary structure. This pipeline includes processing mutated FASTA file of protein primary sequence data, submitting sequence to LOMEST and TASSER prediction server to get predicted models, use Swiss-PDB viewer to manipulate and visualize models, superpose protein models, calculate RMS between models globally and locally. We also developed R pipeline for alignment, superposition, RMSD calculation, clustering of structure models.

3.	Pipeline for processing and analyzing Long non-coding RNAs(LncRNAs)
We develop this pipeline for processing and analyzing Downstream of Gene-containing transcript(DoGs) sequence data. This pipeline includes downloading FASTQ files, aligning short reads on the specified reference genome, collecting intergenic reads, calculating coverage of 5kb and 10kb downstream region of each transcript, identifying DoGs endpoints, comparing DoGs endpoints between two conditions, and differential analysis on DoGs region.

4.	Pipeline for identifying Alternative Polyadenylation(APA) from RNA-Seq data
We develop this pipeline to study the effect of 3′ UTR shortening or lengthening on gene expression. This pipeline includes wrapping DaPars software and InPAS to identify Alternative Polyadenylation site from RNA-Seq data.


5.	PathwaySplice R package
We develop this R package to perform unbiased pathway enrichment analysis when using differential exons, splice junction, exon and splice junction usage based results.

6.	GOSJ pipeline
We develop this R pipeline to include differential exon, splice junction, exon and splice junction usage based results, differential gene expression based results, and using rMATs based results together for obtaining comprehensive analysis.

7.	sraDataSubmitter pipeline
We develop this sraDataSubmitter pipeline to make genomic data submission to SRA automatically. This pipeline includes creating the metadata files(Model.organism.animal.1.0.xlsx and SRA_metadata_acc.xlsx ) for the samples, downloading and installing Aspera Connect software and automatic data submission.

8.	flowR pipeline
We develop this flowR pipeline to process and analyze flow cytometry data.

9.	Sophia pipeline
We develop this Sophia R pipeline to process and analyze microarray based gene expression data, use the differential gene list to perform GSEA analysis.

10.	callSomaticVariation pipeline
We develop this pipeline to use strelka and mutect to identify somatic variants, and to use vcftools to process vcf files, and to use annovar and VEP to annotate variants.    

11.	ATAC-seq pipeline
We have downloaded and installed ATAC-seq procedures from https://github.com/kundajelab/atac_dnase_pipelines. The testing of this pipeline in our this pipeline in our system is under way.

12. Pipeline to study detained introns related RNA-Seq data
