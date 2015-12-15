# WGS-analysis
Basically, WGS=whole genome sequencing, usually the first file we obtained is the fastq file. If it is single-end read, then one file will be obtained. For paired-end reads, two fastq will be obtained. Usually these two files are marked as filename.end1.fq and filename.end.fq. In bwa, one will be called read.fq and the other is mates.fq. (how these two files corresponding, need to set up -p flag when use bwa for alignment).
####Basic workflow
fastq files--(bwa)--sam file--(samtools)--bam file--(samtools)--sorted bam file--(add filter or do annotation)--(SV detection tools)--vcf or other format files



