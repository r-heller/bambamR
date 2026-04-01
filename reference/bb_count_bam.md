# Count Reads in BAM File

Returns the total number of reads in a BAM file using Rsamtools or
system samtools.

## Usage

``` r
bb_count_bam(path)
```

## Arguments

- path:

  Character. Path to a BAM file.

## Value

An integer: total number of reads.

## Examples

``` r
# \donttest{
# count <- bb_count_bam("aligned.bam")
# }
```
