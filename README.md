# SpatialCTD v1

## SpatialCTD: a large-scale TME spatial transcriptomic dataset to evaluate cell type deconvolution for immuno-oncology. [[paper]](https://www.biorxiv.org/content/10.1101/2023.04.11.536333v1)[[supplementary]](https://www.biorxiv.org/content/10.1101/2023.04.11.536333v1.supplementary-material)

SpatialCTD is a large-scale spatial transcriptomic dataset encompassing 1.8 million cells from the human tumor microenvironment across the lung, kidney, and liver. The ST datasets used for CTD in SpatialCTD v1 are generated from real spatial transcriptomic datasets via gridded spots method. 

For each sample in SpatialCTD, it includes:
- Spot location file: contains the spatial information of each pseudo spot.
- Spot gene expression file: provides spot-level gene expression data.
- Ground truth file: contains the cell type proportion per pseudo spot.
- Cell mapping file: displays the mapping relationship between the pseudo spot ID and the cell ID.

The dataset generation workflow and summary are as follows:

<img src="/images/figure_1_dataset.jpg" alt="pdf-image" width="50%">
For thorough details, see the preprint: [[Biorxiv]](https://www.biorxiv.org/content/10.1101/2023.04.11.536333v1)


