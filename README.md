Computational methods for single cell RNA and genome assembly resolution using genetic variation

New sequencing technologies have driven biological research in the past several decades allowing for highly accurate measurements of genomes and transcriptomes. But much of the complexity of these systems is still out of our reach. Here I use properties of genetic variation in samples to uncover some of these features.

Single cell RNA-seq (scRNAseq) has revolutionized transcriptomics by enabling researchers to measure the transcriptional landscape at the cellular level instead of an average transcript level across all of the varied cells and cell types in the sample.
But several factors make the interpretation of these experiments challenging.
Due to the Poisson loading process of the cells into the nanodroplets, as well as the random sampling of a finite barcode set, some barcodes represent multiple cells. Cells may lyse in solution before the droplet partitioning is done which means that some measured RNA will come from this ambient RNA source and not the cell of interest.
And finallly, these other technical artifacts  make comparing scRNAseq results across multiple experiments difficult.
Multiplexing cells from multiple individual into the same experiment can help solve these problems by providing additional comparative information.
This then introduces a further problem---the need to demultiplex the samples from this mixture.
I describe a method using Bayesian deconvolution that for exploits the genetic variation between individuals to deconvolve the cells to their individual of origin, detect doublet cell barcodes, and measure the amount of ambient RNA in the system.

While the technology improvements and cost reductions of third generation long read sequencing techniques have revolutionized genome assembly, problems remain especially for certain challenging organisms such as those that are very small or highly heterozygous.
When assembling a genome, reads with inexact matches must be determined to have arisen from sequencing errors, paralogous repeat sequences from different regions of the genome, or from the differences between haplotypes.
Until recently, relatively high DNA input requirements (e.g. 5$\mu$g) have made long read sequencing out of reach for single individuals of small organisms.
One solution to this is to sequence a mixture of DNA from multiple individuals.
However, this further exacerbates the problem of heterozygosity in the assembly process as there are then many more than two haplotypes.
I demonstrate how a new low-input library prep can be used to create a high quality assembly of a single \textit{Anopheles coluzzii} genome and compare it to the current PEST reference genome for the closely related \textit{Anopheles gambiae} species.
Continuing to address the remaining problems with genome assembly in the modern era, I propose a new approach that uses the heterozygous genetic variation in a diploid sample to improve the assembly of both haplotypes.
This uses phasing consistency of heterozygous loci as a signal for physical linkage, and can combine information from high quality long reads, linked reads, and Hi-C technologies.
Based on this approach I describe a suite of methods for phased genome assembly, haplotype phasing of existing assemblies, and phasing aware assembly scaffolding.
