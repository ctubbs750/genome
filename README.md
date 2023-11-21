# Snakemake workflow: genome

A Snakemake workflow for installing a reference genome along with its supporting files.

# Usage

This workflow is designed to be incorporated into an existing Snakemake pipeline for integrative analysis. To use it, you can point towards its Snakefile raw url during module import. By default, it will install the hg38 human reference genome into the existing project directory under:

 `/resources/data/genome/{build}`

To modify either component, first create a module specific config. Accepted parameters are:
- "INSTALL_DIR". Path to desired installation directory.
- "GENOME_BUILDS".  List of strings(i.e. "hg19", "hg38") in json or yaml format. 