# fast_genome_variants
A tool for calling all types of variants!

DISCLAIMER: This tool/README is for CWL lessons only. There is actually no tool.

## Getting Started

```
git clone https://github.com/bcosc/fast_genome_variants.git
make
./fgv haplotype -input sample.bam -output sample.haplotype.vcf
./fgv joint_haplotype -input sample.bam -input sample2.bam -output sample.haplotype.vcf
```

## Tool Requirements

FGV requires 2GB RAM as a base requirement for running. When running with joint_haplotype, FGV requires 2GB RAM for each BAM input. Each BAM must be indexed, FGV does not create indexes.
