# fast_genome_variants
A tool for calling all types of variants!

DISCLAIMER: This tool/README is for CWL lessons only. There is actually no tool.

## Getting Started

```
git clone https://github.com/bcosc/fast_genome_variants.git
make
./fgv haplotype -input sample.bam -output sample.haplotype.vcf
./fgv joint_haplotype -input sample.bam -input sample2.bam -output sample.haplotype.vcf
./fgv structural -input sample.bam -output sample.structural.vcf
```

## Tool Requirements

FGV requires 2GB RAM as a base requirement for running. When running with joint_haplotype, FGV requires 2GB RAM and 1 CPU for each BAM input. Each BAM must also be indexed, FGV does not create indexes.

When calling structural variants, the input bam and index must by in the output directory or else the variant caller will not be able to process it.

## Optional tool Arguments

-GVCF | Create a GVCF instead of VCF
-intervals [chr1:1-10000] | Choose an interval to call variants
