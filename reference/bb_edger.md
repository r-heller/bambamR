# Differential Expression with edgeR

Runs edgeR quasi-likelihood differential expression analysis. Requires
the `edgeR` package.

## Usage

``` r
bb_edger(counts, group, design = NULL)
```

## Arguments

- counts:

  Numeric matrix. Raw count matrix.

- group:

  Factor or character vector. Group assignment for each sample.

- design:

  A design matrix. If `NULL`, a simple group design is created.

## Value

A data.frame with columns `gene`, `log2fc`, `pvalue`, `padj`.

## Examples

``` r
# \donttest{
if (requireNamespace("edgeR", quietly = TRUE)) {
  counts <- matrix(rpois(600, 100), nrow = 100, ncol = 6,
    dimnames = list(paste0("gene", 1:100), paste0("S", 1:6)))
  group <- factor(rep(c("ctrl", "treat"), each = 3))
  result <- bb_edger(counts, group)
  head(result)
}
#>    gene      log2fc    pvalue      padj
#> 1 gene1  0.03671007 0.7384657 0.9569110
#> 2 gene2 -0.03459959 0.7565418 0.9569110
#> 3 gene3  0.05703588 0.6369106 0.9368175
#> 4 gene4 -0.05426327 0.6554927 0.9368175
#> 5 gene5  0.16544791 0.1808408 0.8209521
#> 6 gene6 -0.06047012 0.5845544 0.9368175
# }
```
