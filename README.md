## Overview

This repo is intended to document the basic usage and output format of [MAGEE](https://github.com/large-scale-gxe-methods/MAGEE)
better than [their own docs](https://github.com/large-scale-gxe-methods/MAGEE/blob/master/inst/doc/MAGEE.pdf), which have a number of
issues including "being a PDF that's hard to copy code blocks from" and "forgetting some steps and not actually working as written".

## Files

- [`renv.lock`](renv.lock): renv lockfile. Run `renv::activate(); renv::restore()` to install all
  required dependencies for MAGEE.
- [`test_magee.Rmd`](test_magee.Rmd): Notebook that runs though slightly-modified examples from
  [`MAGEE.pdf`](https://github.com/large-scale-gxe-methods/MAGEE/blob/master/inst/doc/MAGEE.pdf)
  and generates the below output files.
- [`magee_gds_out.tsv`](magee_gds_out.tsv): Output from `glmm.gei()`.
- [`magee_meta.tsv`](magee_meta.tsv): Output from `glmm.gei.meta()`.
- [`magee_magee.tsv`](magee_magee.tsv): Output from `MAGEE()`, via `data.table::fwrite()`.
