# Package index

## Data Import

Read FASTQ and BAM files into R.

- [`bb_read_fastq()`](https://r-heller.github.io/bambamR/reference/bb_read_fastq.md)
  : Read FASTQ Files
- [`bb_read_bam()`](https://r-heller.github.io/bambamR/reference/bb_read_bam.md)
  : Read BAM Files
- [`bb_count_bam()`](https://r-heller.github.io/bambamR/reference/bb_count_bam.md)
  : Count Reads in BAM File

## Quality Control

Compute and visualize QC metrics from sequencing data.

- [`bb_qc()`](https://r-heller.github.io/bambamR/reference/bb_qc.md) :
  Generate QC Metrics
- [`bb_qc_summary()`](https://r-heller.github.io/bambamR/reference/bb_qc_summary.md)
  : QC Summary
- [`bb_plot_qc()`](https://r-heller.github.io/bambamR/reference/bb_plot_qc.md)
  : QC Visualization Panel

## Alignment & Counting

Align reads to a reference genome and count per-gene overlaps.

- [`bb_align()`](https://r-heller.github.io/bambamR/reference/bb_align.md)
  : Align Reads to Reference Genome
- [`bb_count_reads()`](https://r-heller.github.io/bambamR/reference/bb_count_reads.md)
  : Count Reads per Gene/Feature

## Normalization

Normalize raw count matrices (CPM, TPM, TMM, RLE).

- [`bb_normalize()`](https://r-heller.github.io/bambamR/reference/bb_normalize.md)
  : Normalize Count Matrix

## Differential Expression

Wrappers for DESeq2, edgeR, and limma-voom that return standardized
results.

- [`bb_deseq2()`](https://r-heller.github.io/bambamR/reference/bb_deseq2.md)
  : Differential Expression with DESeq2
- [`bb_edger()`](https://r-heller.github.io/bambamR/reference/bb_edger.md)
  : Differential Expression with edgeR
- [`bb_limma_voom()`](https://r-heller.github.io/bambamR/reference/bb_limma_voom.md)
  : Differential Expression with limma-voom

## Visualization

Publication-ready plots. Every function returns a ggplot2 object.

- [`bb_oncoplot()`](https://r-heller.github.io/bambamR/reference/bb_oncoplot.md)
  : Create Publication-Ready Oncoplot
- [`bb_volcano()`](https://r-heller.github.io/bambamR/reference/bb_volcano.md)
  : Volcano Plot
- [`bb_heatmap()`](https://r-heller.github.io/bambamR/reference/bb_heatmap.md)
  : Heatmap of Top Differentially Expressed Genes
- [`bb_pca()`](https://r-heller.github.io/bambamR/reference/bb_pca.md) :
  PCA Plot
- [`bb_ma_plot()`](https://r-heller.github.io/bambamR/reference/bb_ma_plot.md)
  : MA Plot

## Pipeline & Export

Run the full end-to-end pipeline and export results.

- [`bb_pipeline()`](https://r-heller.github.io/bambamR/reference/bb_pipeline.md)
  : Run Full bambamR Pipeline
- [`bb_export_rds()`](https://r-heller.github.io/bambamR/reference/bb_export_rds.md)
  : Export Results to RDS
- [`bb_export_csv()`](https://r-heller.github.io/bambamR/reference/bb_export_csv.md)
  : Export DE Results to CSV
- [`bb_export_tsv()`](https://r-heller.github.io/bambamR/reference/bb_export_tsv.md)
  : Export DE Results to TSV
- [`bb_run_app()`](https://r-heller.github.io/bambamR/reference/bb_run_app.md)
  : Launch bambamR Shiny App

## Example Data

Bundled datasets for exploring every feature without external files.

- [`bb_example_counts()`](https://r-heller.github.io/bambamR/reference/bb_example_counts.md)
  : Load Example Count Matrix
- [`bb_example_mutations()`](https://r-heller.github.io/bambamR/reference/bb_example_mutations.md)
  : Load Example Mutation Data
- [`bb_example_de()`](https://r-heller.github.io/bambamR/reference/bb_example_de.md)
  : Load Example DE Results

## Classes & Methods

S3 classes for pipeline results and QC objects.

- [`print(`*`<bb_result>`*`)`](https://r-heller.github.io/bambamR/reference/print.bb_result.md)
  : Print method for bb_result
- [`print(`*`<bb_qc>`*`)`](https://r-heller.github.io/bambamR/reference/print.bb_qc.md)
  : Print method for bb_qc
- [`summary(`*`<bb_qc>`*`)`](https://r-heller.github.io/bambamR/reference/summary.bb_qc.md)
  : Summary method for bb_qc
- [`bambamR`](https://r-heller.github.io/bambamR/reference/bambamR-package.md)
  [`bambamR-package`](https://r-heller.github.io/bambamR/reference/bambamR-package.md)
  : bambamR: End-to-End RNA-Seq Processing from FASTQ to
  Publication-Ready Plots
