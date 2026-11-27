# upstart-task-03-analysis-pipeline
Reproducible, single-command bioinformatics analysis pipeline chaining multi-step sequence filtering, metric computation, and reporting with centralized top-level parameters and preserved intermediate files
# Task 03: Multiple Sequence Alignment (MSA)

Multiple sequence alignment of `seq1_example_query` (`Query_1530695`, 60 bp) against top *Homo sapiens* *HBB* (hemoglobin subunit beta) BLAST hits using NCBI BLASTN (`RID: GJCU4FGN014`, `core_nt`) and NCBI MSA Viewer.

## Alignment & Workflow Summary

* **Query Sequence:** `seq1_example_query` (`Query_1530695`, 60 bp DNA fragment)
* **Aligned Sequences:** `Query_1530695` alongside top *Homo sapiens* subject sequences (`LC836263.1`, `MK476479.1`, `LC772513.1`, `MK476473.1`, `MK476391.1`, `MK476368.1`, `MK476341.1`, `MK476238.1`)
* **Tools Used:** NCBI BLAST (`blastn` against `core_nt`) and NCBI MSA Viewer (`1.26.0`)
* **Alignment File:** Uploaded alignment file exported from NCBI MSA Viewer
* **Key Observations:** All 60 nucleotide positions (`1..60`) align cleanly across the displayed *Homo sapiens* hits with 100% identity across the aligned window (`100%` query coverage, `100.00%` identity, E-value `6e-21`), while subject sequences vary in total length and starting coordinates.

## Biological Interpretation

The complete base-by-base alignment across all 60 positions of `Query_1530695` with *Homo sapiens* *HBB* (hemoglobin subunit beta) sequences shows strong sequence conservation across this region of the human beta-globin locus. Because hemoglobin subunit beta forms part of adult hemoglobin A responsible for oxygen transport in red blood cells, this conserved match reflects shared *HBB* sequence identity across the aligned segment. However, because the alignment covers a short 60 bp fragment rather than a full-length gene or transcript, identical matches over this short window cannot distinguish specific variants, alleles, or full transcript isoforms without longer sequences and functional context.
