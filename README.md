# Analysing the protein-DNA binding sites in _Arabidopsis thaliana_ from ChIP-seq experiments

## [ArabidopsisGenome](ArabidopsisGenome)

This folder contains the files used in this work, which contain all the information collected from different public resources and bibliography on the genes, genome, gaps and enhancers of _Arabidoposis thaliana_, assembly TAIR10. 

1. [listFirstGenes.PY](ArabidopsisGenome/listFirstGenes.py)
    * List of genes obtained directly from the [Ensembl plants Biomart](https://plants.ensembl.org/index.html) search tool. These genes belong to chr1, chr2, chr3, chr4, chr5, chrMt and chrPt.
2. [listProcessGenes.txt](ArabidopsisGenome/listProcessGenes.txt)
    * List of genes in the above file with their corresponding canonical transcript ID according to the Ensembl plants database.
3. [dataGeneModel.gff3](ArabidopsisGenome/dataGeneModel.gff3)
    * A tab-delimited text file containing information about the gene, transcript and exons of each of the processed genes.
4. [enhancersRaw.txt](ArabidopsisGenome/enhancersRaw.txt)
    * List of enhancers obtained in the work of [Zhu,B et al](https://academic.oup.com/plcell/article/27/9/2415/6206353).
5. [gaps.txt](ArabidopsisGenome/gaps.txt)
    * File extracted directly from the [UCSC](https://genome.ucsc.edu/goldenPath/help/examples/hubExamples/hubAssembly/plantAraTha1/araTha1/gap.html) resource containing all the gaps of the genome under study. 
6. [gapsTair10.py](ArabidopsisGenome/gapsTair10.py)
    * File derived from the previous one containing the gaps of the genome under study with a length greater than 10 nucleotides.

### [Processed](ArabidopsisGenome/Processed)

This folder contains the gene models gathered by chromosome, describing the extent of their genomic features for the selected transcript.

1. [gene\_chr1\_processed.bed](ArabidopsisGenome/Processed/gene_chr1_processed.bed)
2. [gene\_chr2\_processed.bed](ArabidopsisGenome/Processed/gene_chr2_processed.bed)
3. [gene\_chr3\_processed.bed](ArabidopsisGenome/Processed/gene_chr3_processed.bed)
4. [gene\_chr4\_processed.bed](ArabidopsisGenome/Processed/gene_chr4_processed.bed)
5. [gene\_chr5\_processed.bed](ArabidopsisGenome/Processed/gene_chr5_processed.bed)
6. [gene\_chrMt\_processed.bed](ArabidopsisGenome/Processed/gene_chrMt_processed.bed)
7. [gene\_chrPt\_processed.bed](ArabidopsisGenome/Processed/gene_chrPt_processed.bed)

### [BM3120](ArabidopsisGenome/BM3120)

#### [7dm](ArabidopsisGenome/BM3120/7dm)

This folder containing the background models for the genome model with 7 kinds of genomic features {promoter>proximal>cleavage>splice>exon>intron>intergenic}.

1. [annotated\_genome\_both\_model.txt](ArabidopsisGenome/BM3120/7dm/annotated_genome_both_model.txt)
    * A tab-delimited text file for both strands with the binding sites annotated by chromosome
2. [count\_genome\_both\_model.txt](ArabidopsisGenome/BM3120/7dm/count_genome_both_model.txt)
    * A tab-delimited text file for both strands with the annotated binding sites count by each type of genomic feature and chromosome

##### [GM](ArabidopsisGenome/BM3120/7dm/GM)

1. [count\_gene\_model.txt](ArabidopsisGenome/BM3120/7dm/GM/count_gene_model.txt)
    * A tab-delimited text file with the annotated binding sites count by each type of genomic feature for every background gene

###### [AnnotatedGenes](ArabidopsisGenome/BM3120/7dm/GM/AnnotatedGenes)

This folder containing the background genes gathered by chromosome

1. [gene\_chr1\_annotated.txt](ArabidopsisGenome/BM3120/7dm/GM/AnnotatedGenes/gene_chr1_annotated.txt)
2. [gene\_chr2\_annotated.txt](ArabidopsisGenome/BM3120/7dm/GM/AnnotatedGenes/gene_chr2_annotated.txt)
3. [gene\_chr3\_annotated.txt](ArabidopsisGenome/BM3120/7dm/GM/AnnotatedGenes/gene_chr3_annotated.txt)
4. [gene\_chr4\_annotated.txt](ArabidopsisGenome/BM3120/7dm/GM/AnnotatedGenes/gene_chr4_annotated.txt)
5. [gene\_chr5\_annotated.txt](ArabidopsisGenome/BM3120/7dm/GM/AnnotatedGenes/gene_chr5_annotated.txt)

#### [8dm](ArabidopsisGenome/BM3120/8dm)

This folder containing the background models for the genome model with 8 kinds of genomic features {promoter>proximal>enhancer>cleavage>splice>exon>intron>intergenic}.

1. [annotated\_genome\_both\_model.txt](ArabidopsisGenome/BM3120/8dm/annotated_genome_both_model.txt)
    * A tab-delimited text file for both strands with the binding sites annotated by chromosome
2. [count\_genome\_both\_model.txt](ArabidopsisGenome/BM3120/8dm/count_genome_both_model.txt)
    * A tab-delimited text file for both strands with the annotated binding sites count by each type of genomic feature and chromosome

##### [PeakEnhancers](ArabidopsisGenome/BM3120/8dm/PeakEnhancers)

This folder containing the annotated enhancers regions gathered by chromosome

1. [enhancer\_chr1\_peaks.txt](ArabidopsisGenome/BM3120/8dm/PeakEnhancers/enhancer_chr1_peaks.txt)
2. [enhancer\_chr2\_peaks.txt](ArabidopsisGenome/BM3120/8dm/PeakEnhancers/enhancer_chr2_peaks.txt)
3. [enhancer\_chr3\_peaks.txt](ArabidopsisGenome/BM3120/8dm/PeakEnhancers/enhancer_chr3_peaks.txt)
4. [enhancer\_chr4\_peaks.txt](ArabidopsisGenome/BM3120/8dm/PeakEnhancers/enhancer_chr4_peaks.txt)
5. [enhancer\_chr5\_peaks.txt](ArabidopsisGenome/BM3120/8dm/PeakEnhancers/enhancer_chr5_peaks.txt)

## [Remap2020](Remap2020)

This folder containing all the raw peaks corresponding to the protein DET1 and cell line Col-0-seedling collected from [Remap2020](https://remap2020.univ-amu.fr/).

1. [remap2020\_DET1\_all\_macs2\_TAIR10\_v1\_0.bed.gz](Remap2020/remap2020_DET1_all_macs2_TAIR10_v1_0.bed.gz) (zip file)
2. [remap2020\_DET1\_all\_macs2\_TAIR10\_v1\_0.bed](Remap2020/remap2020_DET1_all_macs2_TAIR10_v1_0.bed)

### [Standardised3120](Remap2020/Standardised3120)

This folder containing all the standardized peaks with a peak_length = 31

1. [DET1\_chr1\_standardised.bed](Remap2020/Standardised3120/DET1_chr1_standardised.bed)
2. [DET1\_chr2\_standardised.bed](Remap2020/Standardised3120/DET1_chr2_standardised.bed)
3. [DET1\_chr3\_standardised.bed](Remap2020/Standardised3120/DET1_chr3_standardised.bed)
4. [DET1\_chr4\_standardised.bed](Remap2020/Standardised3120/DET1_chr4_standardised.bed)
5. [DET1\_chr5\_standardised.bed](Remap2020/Standardised3120/DET1_chr5_standardised.bed)


## [DET1](DET1) 

This folder containing all the annotated ChIPseq models and their corresponding analyses for this target protein

### [7dm](DET1/7dm)

#### [GSE112951](DET1/7dm/GSE112951)

This folder containing the annotated ChIPseq models through the corresponding background model with the peak_length = 31 and rate_overlap = 0.2

##### [5d-D](DET1/7dm/GSE112951/5d-D)

1. [annotated\_peaks\_GSE112951\_Col-0-seedling\_5d-D\_both\_region.txt](DET1/7dm/GSE112951/5d-D/annotated_peaks_GSE112951_Col-0-seedling_5d-D_both_region.txt)
2. [counting\_GSE112951\_Col-0-seedling\_5d-D\_both\_region.txt](DET1/7dm/GSE112951/5d-D/counting_GSE112951_Col-0-seedling_5d-D_both_region.txt)
3. [characteristic\_profile\_GSE112951\_Col-0-seedling\_5d-D\_both\_region.txt](DET1/7dm/GSE112951/5d-D/characteristic_profile_GSE112951_Col-0-seedling_5d-D_both_region.txt)
4. [goodness\_test\_GSE112951\_Col-0-seedling\_5d-D\_both\_region.txt](DET1/7dm/GSE112951/5d-D/goodness_test_GSE112951_Col-0-seedling_5d-D_both_region.txt)

###### [Figures](DET1/7dm/GSE112951/5d-D/Figures)

1. [grid\_relatFreq\_zScores\_GSE112951\_Col-0-seedling\_5d-D\_region.pdf](DET1/7dm/GSE112951/5d-D/Figures/grid_relatFreq_zScores_GSE112951_Col-0-seedling_5d-D_region.pdf)
2. [relativeFreq\_GSE112951\_Col-0-seedling\_5d-D\_both\_region.pdf](DET1/7dm/GSE112951/5d-D/Figures/relativeFreq_GSE112951_Col-0-seedling_5d-D_both_region.pdf)
3. [zScores\_GSE112951\_Col-0-seedling\_5d-D\_both\_region.pdf](DET1/7dm/GSE112951/5d-D/Figures/zScore_GSE112951_Col-0-seedling_5d-D_both_region.pdf)

##### [5d-L](DET1/7dm/GSE112951/5d-L)

1. [annotated\_peaks\_GSE112951\_Col-0-seedling\_5d-L\_both\_region.txt](DET1/7dm/GSE112951/5d-L/annotated_peaks_GSE112951_Col-0-seedling_5d-L_both_region.txt)
2. [counting\_GSE112951\_Col-0-seedling\_5d-L\_both\_region.txt](DET1/7dm/GSE112951/5d-L/counting_GSE112951_Col-0-seedling_5d-L_both_region.txt)
3. [characteristic\_profile\_GSE112951\_Col-0-seedling\_5d-L\_both\_region.txt](DET1/7dm/GSE112951/5d-L/characteristic_profile_GSE112951_Col-0-seedling_5d-L_both_region.txt)
4. [goodness\_test\_GSE112951\_Col-0-seedling\_5d-L\_both\_region.txt](DET1/7dm/GSE112951/5d-L/goodness_test_GSE112951_Col-0-seedling_5d-L_both_region.txt)

###### [Figures](DET1/7dm/GSE112951/5d-L/Figures)

1. [grid\_relatFreq\_zScores\_GSE112951\_Col-0-seedling\_5d-L\_region.pdf](DET1/7dm/GSE112951/5d-L/Figures/grid_relatFreq_zScores_GSE112951_Col-0-seedling_5d-L_region.pdf)
2. [relativeFreq\_GSE112951\_Col-0-seedling\_5d-L\_both\_region.pdf](DET1/7dm/GSE112951/5d-L/Figures/relativeFreq_GSE112951_Col-0-seedling_5d-L_both_region.pdf)
3. [zScores\_GSE112951\_Col-0-seedling\_5d-L\_both\_region.pdf](DET1/7dm/GSE112951/5d-L/Figures/zScore_GSE112951_Col-0-seedling_5d-L_both_region.pdf)

##### [det1\_5d-D](DET1/7dm/GSE112951/det1_5d-D)

1. [annotated\_peaks\_GSE112951\_Col-0-seedling\_det1\_5d-D\_both\_region.txt](DET1/7dm/GSE112951/det1_5d-D/annotated_peaks_GSE112951_Col-0-seedling_det1_5d-D_both_region.txt)
2. [counting\_GSE112951\_Col-0-seedling\_det1\_5d-D\_both\_region.txt](DET1/7dm/GSE112951/det1_5d-D/counting_GSE112951_Col-0-seedling_det1_5d-D_both_region.txt)
3. [characteristic\_profile\_GSE112951\_Col-0-seedling\_det1\_5d-D\_both\_region.txt](DET1/7dm/GSE112951/det1_5d-D/characteristic_profile_GSE112951_Col-0-seedling_det1_5d-D_both_region.txt)
4. [goodness\_test\_GSE112951\_Col-0-seedling\_det1\_5d-D\_both\_region.txt](DET1/7dm/GSE112951/det1_5d-D/goodness_test_GSE112951_Col-0-seedling_det1_5d-D_both_region.txt)

###### [Figures](DET1/7dm/GSE112951/det1_5d-D/Figures)

1. [grid\_relatFreq\_zScores\_GSE112951\_Col-0-seedling\_det1\_5d-D\_region.pdf](DET1/7dm/GSE112951/det1_5d-D/Figures/grid_relatFreq_zScores_GSE112951_Col-0-seedling_det1_5d-D_region.pdf)
2. [relativeFreq\_GSE112951\_Col-0-seedling\_det1\_5d-D\_both\_region.pdf](DET1/7dm/GSE112951/det1_5d-D/Figures/relativeFreq_GSE112951_Col-0-seedling_det1_5d-D_both_region.pdf)
3. [zScores\_GSE112951\_Col-0-seedling\_det1\_5d-D\_both\_region.pdf](DET1/7dm/GSE112951/det1_5d-D/Figures/zScore_GSE112951_Col-0-seedling_det1_5d-D_both_region.pdf)


##### [det1\_5d-L](DET1/7dm/GSE112951/det1_5d-L)

1. [annotated\_peaks\_GSE112951\_Col-0-seedling\_det1\_5d-L\_both\_region.txt](DET1/7dm/GSE112951/det1_5d-L/annotated_peaks_GSE112951_Col-0-seedling_det1_5d-L_both_region.txt)
2. [counting\_GSE112951\_Col-0-seedling\_det1\_5d-L\_both\_region.txt](DET1/7dm/GSE112951/det1_5d-L/counting_GSE112951_Col-0-seedling_det1_5d-L_both_region.txt)
3. [characteristic\_profile\_GSE112951\_Col-0-seedling\_det1\_5d-L\_both\_region.txt](DET1/7dm/GSE112951/det1_5d-L/characteristic_profile_GSE112951_Col-0-seedling_det1_5d-L_both_region.txt)
4. [goodness\_test\_GSE112951\_Col-0-seedling\_det1\_5d-L\_both\_region.txt](DET1/7dm/GSE112951/det1_5d-L/goodness_test_GSE112951_Col-0-seedling_det1_5d-L_both_region.txt)

###### [Figures](DET1/7dm/GSE112951/det1_5d-L/Figures)

1. [grid\_relatFreq\_zScores\_GSE112951\_Col-0-seedling\_det1\_5d-L\_region.pdf](DET1/7dm/GSE112951/det1_5d-L/Figures/grid_relatFreq_zScores_GSE112951_Col-0-seedling_det1_5d-L_region.pdf)
2. [relativeFreq\_GSE112951\_Col-0-seedling\_det1\_5d-L\_both\_region.pdf](DET1/7dm/GSE112951/det1_5d-L/Figures/relativeFreq_GSE112951_Col-0-seedling_det1_5d-L_both_region.pdf)
3. [zScores\_GSE112951\_Col-0-seedling\_det1\_5d-L\_both\_region.pdf](DET1/7dm/GSE112951/det1_5d-L/Figures/zScore_GSE112951_Col-0-seedling_det1_5d-L_both_region.pdf)

##### [Analysis](DET1/7dm/GSE112951/Analysis)

A folder containing the comparisons between the different ChIPseq model pairs for the background model with 7 dimensions

1. [homogeneity\_test\_Col-0-seedling\_DET1-5d-D\_DET1-det1\_5d-L\_both\_region.txt](DET1/7dm/GSE112951/Analysis/homogeneity_test_Col-0-seedling_DET1-5d-D_DET1-det1_5d-L_both_region.txt)
2. [homogeneity\_test\_Col-0-seedling\_DET1-5d-D\_DET1-det1\_5d-D\_both\_region.txt](DET1/7dm/GSE112951/Analysis/homogeneity_test_Col-0-seedling_DET1-5d-D_DET1-det1_5d-D_both_region.txt)
3. [homogeneity\_test\_Col-0-seedling\_DET1-5d-L\_DET1-5d-D\_both\_region.txt](DET1/7dm/GSE112951/Analysis/homogeneity_test_Col-0-seedling_DET1-5d-L_DET1-5d-D_both_region.txt)
4. [homogeneity\_test\_Col-0-seedling\_DET1-5d-L\_DET1-det1\_5d-L\_both\_region.txt](DET1/7dm/GSE112951/Analysis/homogeneity_test_Col-0-seedling_DET1-5d-L_DET1-det1_5d-L_both_region.txt)
5. [homogeneity\_test\_Col-0-seedling\_DET1-5d-L\_DET1-det1\_5d-D\_both\_region.txt](DET1/7dm/GSE112951/Analysis/homogeneity_test_Col-0-seedling_DET1-5d-L_DET1-det1_5d-D_both_region.txt)
6. [homogeneity\_test\_Col-0-seedling\_DET1-det1\_5d-D\_DET1-det1\_5d-L\_both\_region.txt](DET1/7dm/GSE112951/Analysis/homogeneity_test_Col-0-seedling_DET1-det1_5d-D_DET1-det1_5d-L_both_region.txt)
7. [statistics_homogeneity\_Col-0-seedling\_DET1-5d-D\_DET1-det1\_5d-L\_both\_region.txt](DET1/7dm/GSE112951/Analysis/statistics_homogeneity_Col-0-seedling_DET1-5d-D_DET1-det1_5d-L_both_region.txt)
8. [statistics_homogeneity\_Col-0-seedling\_DET1-5d-D\_DET1-det1\_5d-D\_both\_region.txt](DET1/7dm/GSE112951/Analysis/statistics_homogeneity_Col-0-seedling_DET1-5d-D_DET1-det1_5d-D_both_region.txt)
9. [statistics_homogeneity\_Col-0-seedling\_DET1-5d-L\_DET1-5d-D\_both\_region.txt](DET1/7dm/GSE112951/Analysis/statistics_homogeneity_Col-0-seedling_DET1-5d-L_DET1-5d-D_both_region.txt)
10. [statistics_homogeneity\_Col-0-seedling\_DET1-5d-L\_DET1-det1\_5d-L\_both\_region.txt](DET1/7dm/GSE112951/Analysis/statistics_homogeneity_Col-0-seedling_DET1-5d-L_DET1-det1_5d-L_both_region.txt)
11. [statistics_homogeneity\_Col-0-seedling\_DET1-5d-L\_DET1-det1\_5d-D\_both\_region.txt](DET1/7dm/GSE112951/Analysis/statistics_homogeneity_Col-0-seedling_DET1-5d-L_DET1-det1_5d-D_both_region.txt)
12. [statistics_homogeneity\_Col-0-seedling\_DET1-det1\_5d-D\_DET1-det1\_5d-L\_both\_region.txt](DET1/7dm/GSE112951/Analysis/statistics_homogeneity_Col-0-seedling_DET1-det1_5d-L_DET1-det1_5d-D_both_region.txt)

###### [Figures](DET1/7dm/GSE112951/Analysis/Figures)

1. [gridmultipleAccumContrbHomogeneityJoint\_GSE112951\_Col-0-seedling\_both\_region.pdf](DET1/7dm/GSE112951/Analysis/Figures/gridmultipleAccumContrbHomogeneityJoint_GSE112951_Col-0-seedling_both_region.pdf)
2. [accumContrbsquar\_Col-0-seedling\_DET1-5d-D\_DET1-det1\_5d-L\_both\_region.pdf](DET1/7dm/GSE112951/Analysis/Figures/accumContrbSquar_Col-0-seedling_DET1-5d-D_DET1-det1_5d-L_both_region.pdf)
3. [accumContrbsquar\_Col-0-seedling\_DET1-5d-D\_DET1-det1\_5d-D\_both\_region.pdf](DET1/7dm/GSE112951/Analysis/Figures/accumContrbSquar_Col-0-seedling_DET1-5d-D_DET1-det1_5d-D_both_region.pdf)
4. [accumContrbsquar\_Col-0-seedling\_DET1-5d-L\_DET1-5d-D\_both\_region.pdf](DET1/7dm/GSE112951/Analysis/Figures/accumContrbSquar_Col-0-seedling_DET1-5d-L_DET1-5d-D_both_region.pdf)
5. [accumContrbsquar\_Col-0-seedling\_DET1-5d-L\_DET1-det1\_5d-L\_both\_region.pdf](DET1/7dm/GSE112951/Analysis/Figures/accumContrbSquar_Col-0-seedling_DET1-5d-L_DET1-det1_5d-L_both_region.pdf)
6. [accumContrbsquar\_Col-0-seedling\_DET1-5d-L\_DET1-det1\_5d-D\_both\_region.pdf](DET1/7dm/GSE112951/Analysis/Figures/accumContrbSquar_Col-0-seedling_DET1-5d-L_DET1-det1_5d-D_both_region.pdf)
2. [accumContrbsquar\_Col-0-seedling\_DET1-det1\_5d-D\_DET1-det1\_5d-L\_both\_region.pdf](DET1/7dm/GSE112951/Analysis/Figures/accumContrbSquar_Col-0-seedling_DET1-det1_5d-D_DET1-det1_5d-L_both_region.pdf)

### [8dm](DET1/8dm)

#### [GSE112951](DET1/8dm/GSE112951)

This folder containing the annotated ChIPseq models through the corresponding background model with the peak_length = 31 and rate_overlap = 0.2

##### [5d-D](DET1/8dm/GSE112951/5d-D)

1. [annotated\_peaks\_GSE112951\_Col-0-seedling\_5d-D\_both\_region.txt](DET1/8dm/GSE112951/5d-D/annotated_peaks_GSE112951_Col-0-seedling_5d-D_both_region.txt)
2. [counting\_GSE112951\_Col-0-seedling\_5d-D\_both\_region.txt](DET1/8dm/GSE112951/5d-D/counting_GSE112951_Col-0-seedling_5d-D_both_region.txt)
3. [characteristic\_profile\_GSE112951\_Col-0-seedling\_5d-D\_both\_region.txt](DET1/8dm/GSE112951/5d-D/characteristic_profile_GSE112951_Col-0-seedling_5d-D_both_region.txt)
4. [goodness\_test\_GSE112951\_Col-0-seedling\_5d-D\_both\_region.txt](DET1/8dm/GSE112951/5d-D/goodness_test_GSE112951_Col-0-seedling_5d-D_both_region.txt)

###### [Figures](DET1/8dm/GSE112951/5d-D/Figures)

1. [grid\_relatFreq\_zScores\_GSE112951\_Col-0-seedling\_5d-D\_region.pdf](DET1/8dm/GSE112951/5d-D/Figures/grid_relatFreq_zScores_GSE112951_Col-0-seedling_5d-D_region.pdf)
2. [relativeFreq\_GSE112951\_Col-0-seedling\_5d-D\_both\_region.pdf](DET1/8dm/GSE112951/5d-D/Figures/relativeFreq_GSE112951_Col-0-seedling_5d-D_both_region.pdf)
3. [zScores\_GSE112951\_Col-0-seedling\_5d-D\_both\_region.pdf](DET1/8dm/GSE112951/5d-D/Figures/zScore_GSE112951_Col-0-seedling_5d-D_both_region.pdf)

##### [5d-L](DET1/8dm/GSE112951/5d-L)

1. [annotated\_peaks\_GSE112951\_Col-0-seedling\_5d-L\_both\_region.txt](DET1/8dm/GSE112951/5d-L/annotated_peaks_GSE112951_Col-0-seedling_5d-L_both_region.txt)
2. [counting\_GSE112951\_Col-0-seedling\_5d-L\_both\_region.txt](DET1/8dm/GSE112951/5d-L/counting_GSE112951_Col-0-seedling_5d-L_both_region.txt)
3. [characteristic\_profile\_GSE112951\_Col-0-seedling\_5d-L\_both\_region.txt](DET1/8dm/GSE112951/5d-L/characteristic_profile_GSE112951_Col-0-seedling_5d-L_both_region.txt)
4. [goodness\_test\_GSE112951\_Col-0-seedling\_5d-L\_both\_region.txt](DET1/8dm/GSE112951/5d-L/goodness_test_GSE112951_Col-0-seedling_5d-L_both_region.txt)

###### [Figures](DET1/8dm/GSE112951/5d-L/Figures)

1. [grid\_relatFreq\_zScores\_GSE112951\_Col-0-seedling\_5d-L\_region.pdf](DET1/8dm/GSE112951/5d-L/Figures/grid_relatFreq_zScores_GSE112951_Col-0-seedling_5d-L_region.pdf)
2. [relativeFreq\_GSE112951\_Col-0-seedling\_5d-L\_both\_region.pdf](DET1/8dm/GSE112951/5d-L/Figures/relativeFreq_GSE112951_Col-0-seedling_5d-L_both_region.pdf)
3. [zScores\_GSE112951\_Col-0-seedling\_5d-L\_both\_region.pdf](DET1/8dm/GSE112951/5d-L/Figures/zScore_GSE112951_Col-0-seedling_5d-L_both_region.pdf)

##### [det1\_5d-D](DET1/8dm/GSE112951/det1_5d-D)

1. [annotated\_peaks\_GSE112951\_Col-0-seedling\_det1\_5d-D\_both\_region.txt](DET1/8dm/GSE112951/det1_5d-D/annotated_peaks_GSE112951_Col-0-seedling_det1_5d-D_both_region.txt)
2. [counting\_GSE112951\_Col-0-seedling\_det1\_5d-D\_both\_region.txt](DET1/8dm/GSE112951/det1_5d-D/counting_GSE112951_Col-0-seedling_det1_5d-D_both_region.txt)
3. [characteristic\_profile\_GSE112951\_Col-0-seedling\_det1\_5d-D\_both\_region.txt](DET1/8dm/GSE112951/det1_5d-D/characteristic_profile_GSE112951_Col-0-seedling_det1_5d-D_both_region.txt)
4. [goodness\_test\_GSE112951\_Col-0-seedling\_det1\_5d-D\_both\_region.txt](DET1/8dm/GSE112951/det1_5d-D/goodness_test_GSE112951_Col-0-seedling_det1_5d-D_both_region.txt)

###### [Figures](DET1/8dm/GSE112951/det1_5d-D/Figures)

1. [grid\_relatFreq\_zScores\_GSE112951\_Col-0-seedling\_det1\_5d-D\_region.pdf](DET1/8dm/GSE112951/det1_5d-D/Figures/grid_relatFreq_zScores_GSE112951_Col-0-seedling_det1_5d-D_region.pdf)
2. [relativeFreq\_GSE112951\_Col-0-seedling\_det1\_5d-D\_both\_region.pdf](DET1/8dm/GSE112951/det1_5d-D/Figures/relativeFreq_GSE112951_Col-0-seedling_det1_5d-D_both_region.pdf)
3. [zScores\_GSE112951\_Col-0-seedling\_det1\_5d-D\_both\_region.pdf](DET1/8dm/GSE112951/det1_5d-D/Figures/zScore_GSE112951_Col-0-seedling_det1_5d-D_both_region.pdf)


##### [det1\_5d-L](DET1/8dm/GSE112951/det1_5d-L)

1. [annotated\_peaks\_GSE112951\_Col-0-seedling\_det1\_5d-L\_both\_region.txt](DET1/8dm/GSE112951/det1_5d-L/annotated_peaks_GSE112951_Col-0-seedling_det1_5d-L_both_region.txt)
2. [counting\_GSE112951\_Col-0-seedling\_det1\_5d-L\_both\_region.txt](DET1/8dm/GSE112951/det1_5d-L/counting_GSE112951_Col-0-seedling_det1_5d-L_both_region.txt)
3. [characteristic\_profile\_GSE112951\_Col-0-seedling\_det1\_5d-L\_both\_region.txt](DET1/8dm/GSE112951/det1_5d-L/characteristic_profile_GSE112951_Col-0-seedling_det1_5d-L_both_region.txt)
4. [goodness\_test\_GSE112951\_Col-0-seedling\_det1\_5d-L\_both\_region.txt](DET1/8dm/GSE112951/det1_5d-L/goodness_test_GSE112951_Col-0-seedling_det1_5d-L_both_region.txt)

###### [Figures](DET1/8dm/GSE112951/det1_5d-L/Figures)

1. [grid\_relatFreq\_zScores\_GSE112951\_Col-0-seedling\_det1\_5d-L\_region.pdf](DET1/8dm/GSE112951/det1_5d-L/Figures/grid_relatFreq_zScores_GSE112951_Col-0-seedling_det1_5d-L_region.pdf)
2. [relativeFreq\_GSE112951\_Col-0-seedling\_det1\_5d-L\_both\_region.pdf](DET1/8dm/GSE112951/det1_5d-L/Figures/relativeFreq_GSE112951_Col-0-seedling_det1_5d-L_both_region.pdf)
3. [zScores\_GSE112951\_Col-0-seedling\_det1\_5d-L\_both\_region.pdf](DET1/8dm/GSE112951/det1_5d-L/Figures/zScore_GSE112951_Col-0-seedling_det1_5d-L_both_region.pdf)

##### [Analysis](DET1/8dm/GSE112951/Analysis)

A folder containing the comparisons between the different ChIPseq model pairs for the background model with 8 dimensions

1. [homogeneity\_test\_Col-0-seedling\_DET1-5d-D\_DET1-det1\_5d-L\_both\_region.txt](DET1/8dm/GSE112951/Analysis/homogeneity_test_Col-0-seedling_DET1-5d-D_DET1-det1_5d-L_both_region.txt)
2. [homogeneity\_test\_Col-0-seedling\_DET1-5d-D\_DET1-det1\_5d-D\_both\_region.txt](DET1/8dm/GSE112951/Analysis/homogeneity_test_Col-0-seedling_DET1-5d-D_DET1-det1_5d-D_both_region.txt)
3. [homogeneity\_test\_Col-0-seedling\_DET1-5d-L\_DET1-5d-D\_both\_region.txt](DET1/8dm/GSE112951/Analysis/homogeneity_test_Col-0-seedling_DET1-5d-L_DET1-5d-D_both_region.txt)
4. [homogeneity\_test\_Col-0-seedling\_DET1-5d-L\_DET1-det1\_5d-L\_both\_region.txt](DET1/8dm/GSE112951/Analysis/homogeneity_test_Col-0-seedling_DET1-5d-L_DET1-det1_5d-L_both_region.txt)
5. [homogeneity\_test\_Col-0-seedling\_DET1-5d-L\_DET1-det1\_5d-D\_both\_region.txt](DET1/8dm/GSE112951/Analysis/homogeneity_test_Col-0-seedling_DET1-5d-L_DET1-det1_5d-D_both_region.txt)
6. [homogeneity\_test\_Col-0-seedling\_DET1-det1\_5d-D\_DET1-det1\_5d-L\_both\_region.txt](DET1/8dm/GSE112951/Analysis/homogeneity_test_Col-0-seedling_DET1-det1_5d-D_DET1-det1_5d-L_both_region.txt)
7. [statistics_homogeneity\_Col-0-seedling\_DET1-5d-D\_DET1-det1\_5d-L\_both\_region.txt](DET1/8dm/GSE112951/Analysis/statistics_homogeneity_Col-0-seedling_DET1-5d-D_DET1-det1_5d-L_both_region.txt)
8. [statistics_homogeneity\_Col-0-seedling\_DET1-5d-D\_DET1-det1\_5d-D\_both\_region.txt](DET1/8dm/GSE112951/Analysis/statistics_homogeneity_Col-0-seedling_DET1-5d-D_DET1-det1_5d-D_both_region.txt)
9. [statistics_homogeneity\_Col-0-seedling\_DET1-5d-L\_DET1-5d-D\_both\_region.txt](DET1/8dm/GSE112951/Analysis/statistics_homogeneity_Col-0-seedling_DET1-5d-L_DET1-5d-D_both_region.txt)
10. [statistics_homogeneity\_Col-0-seedling\_DET1-5d-L\_DET1-det1\_5d-L\_both\_region.txt](DET1/8dm/GSE112951/Analysis/statistics_homogeneity_Col-0-seedling_DET1-5d-L_DET1-det1_5d-L_both_region.txt)
11. [statistics_homogeneity\_Col-0-seedling\_DET1-5d-L\_DET1-det1\_5d-D\_both\_region.txt](DET1/8dm/GSE112951/Analysis/statistics_homogeneity_Col-0-seedling_DET1-5d-L_DET1-det1_5d-D_both_region.txt)
12. [statistics_homogeneity\_Col-0-seedling\_DET1-det1\_5d-D\_DET1-det1\_5d-L\_both\_region.txt](DET1/8dm/GSE112951/Analysis/statistics_homogeneity_Col-0-seedling_DET1-det1_5d-L_DET1-det1_5d-D_both_region.txt)

###### [Figures](DET1/8dm/GSE112951/Analysis/Figures)

1. [gridmultipleAccumContrbHomogeneityJoint\_GSE112951\_Col-0-seedling\_both\_region.pdf](DET1/8dm/GSE112951/Analysis/Figures/gridmultipleAccumContrbHomogeneityJoint_GSE112951_Col-0-seedling_both_region.pdf)
2. [accumContrbsquar\_Col-0-seedling\_DET1-5d-D\_DET1-det1\_5d-L\_both\_region.pdf](DET1/8dm/GSE112951/Analysis/Figures/accumContrbSquar_Col-0-seedling_DET1-5d-D_DET1-det1_5d-L_both_region.pdf)
3. [accumContrbsquar\_Col-0-seedling\_DET1-5d-D\_DET1-det1\_5d-D\_both\_region.pdf](DET1/8dm/GSE112951/Analysis/Figures/accumContrbSquar_Col-0-seedling_DET1-5d-D_DET1-det1_5d-D_both_region.pdf)
4. [accumContrbsquar\_Col-0-seedling\_DET1-5d-L\_DET1-5d-D\_both\_region.pdf](DET1/8dm/GSE112951/Analysis/Figures/accumContrbSquar_Col-0-seedling_DET1-5d-L_DET1-5d-D_both_region.pdf)
5. [accumContrbsquar\_Col-0-seedling\_DET1-5d-L\_DET1-det1\_5d-L\_both\_region.pdf](DET1/8dm/GSE112951/Analysis/Figures/accumContrbSquar_Col-0-seedling_DET1-5d-L_DET1-det1_5d-L_both_region.pdf)
6. [accumContrbsquar\_Col-0-seedling\_DET1-5d-L\_DET1-det1\_5d-D\_both\_region.pdf](DET1/8dm/GSE112951/Analysis/Figures/accumContrbSquar_Col-0-seedling_DET1-5d-L_DET1-det1_5d-D_both_region.pdf)
2. [accumContrbsquar\_Col-0-seedling\_DET1-det1\_5d-D\_DET1-det1\_5d-L\_both\_region.pdf](DET1/8dm/GSE112951/Analysis/Figures/accumContrbSquar_Col-0-seedling_DET1-det1_5d-D_DET1-det1_5d-L_both_region.pdf)

