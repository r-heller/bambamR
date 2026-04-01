# Count Reads per Gene/Feature

Counts reads overlapping genomic features. Uses
[`GenomicAlignments::summarizeOverlaps()`](https://rdrr.io/pkg/GenomicAlignments/man/summarizeOverlaps-methods.html)
if available, otherwise shells out to `featureCounts` from the Subread
package.

## Usage

``` r
bb_count_reads(
  bam_paths,
  annotation,
  method = c("auto", "internal", "featureCounts"),
  threads = 4L,
  feature_type = "exon",
  attr_type = "gene_id",
  paired = FALSE
)
```

## Arguments

- bam_paths:

  Character vector. Paths to BAM files.

- annotation:

  Character. Path to GTF/GFF annotation file.

- method:

  Character. `"auto"` tries GenomicAlignments first, then featureCounts;
  `"internal"` forces GenomicAlignments; `"featureCounts"` forces the
  external tool.

- threads:

  Integer. Number of threads for featureCounts. Default `4`.

- feature_type:

  Character. Feature type to count (GTF column 3). Default `"exon"`.

- attr_type:

  Character. Attribute to group by. Default `"gene_id"`.

- paired:

  Logical. Paired-end data. Default `FALSE`.

## Value

A numeric matrix of counts (genes x samples). Rownames are gene IDs,
colnames are derived from BAM file names.

## Examples

``` r
# \donttest{
# Requires BAM files and a GTF annotation
# counts <- bb_count_reads(c("s1.bam", "s2.bam"), "genes.gtf")
# }
```
