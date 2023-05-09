# SpatialCTD v1

## SpatialCTD: a large-scale TME spatial transcriptomic dataset to evaluate cell type deconvolution for immuno-oncology. [[paper]](https://www.biorxiv.org/content/10.1101/2023.04.11.536333v1)[[supplementary]](https://www.biorxiv.org/content/10.1101/2023.04.11.536333v1.supplementary-material)


## NEWS
* [04/2023] Human Lung and Liver datasets in SpatialCTD v1 are released!

## GNNDeconvolver Installation and Running

We have made jupiter notebooks with detailed instructions for GNNDeconvolver running. Please refer to the jupiter notebooks under GNNDeconvolver folder.

## SpatialCTD

SpatialCTD is a large-scale spatial transcriptomic dataset encompassing 1.8 million cells from the human tumor microenvironment across the lung, kidney, and liver. The ST datasets used for CTD in SpatialCTD v1 are generated from real spatial transcriptomic datasets via gridded spots method. 

For each sample in SpatialCTD, it includes:
- Spot location file: contains the spatial information of each pseudo spot.
- Spot gene expression file: provides spot-level gene expression data.
- Ground truth file: contains the cell type proportion per pseudo spot.
- Cell mapping file: displays the mapping relationship between the pseudo spot ID and the cell ID.

The dataset generation workflow and summary are as follows:

<img src="/images/figure_1_dataset.jpg" alt="pdf-image" width="50%">

For thorough details, see the preprint: [[Biorxiv]](https://www.biorxiv.org/content/10.1101/2023.04.11.536333v1)


## SpatialCTD online converter Tool
To ease the process of converting spatial transcriptomics data at single-cell resolution to pseudo spots for benchmarking cell type deconvolution, we have developed a web-based online conversion tool. The online converter tool can be accessed at [[website]](https://omicsml.github.io/SpatialCTD/)

A few required inputs are as below:
- Coordinates of single-cell local in FOV file: contains single-cell level coordinates local in field of view (FOV).
- Coordinates of FOV file: indicates the coordinates of FOV in the slide, which is the spatial coordinates of the center point of each FOV.
- Single-cell level gene expression file (optional)
- Single-cell level cell type file (optional)
- FOV size: specifies the pixel size of each FOV
- Pseudo spot split in one FOV: specifies how the spots in the FOV are divided to further defines the size of pseudo spot.

<img src="/images/converter.jpg" alt="pdf-image" width="50%">

## GNNDeconvolver

<img src="/images/GNN.jpg" alt="pdf-image" width="50%">


## Citation

If you find our work useful in your research, please consider citing our SpatialCTD paper:

```bibtex
@article{ding2023spatialctd,
  title={SpatialCTD: a large-scale TME spatial transcriptomic dataset to evaluate cell type deconvolution for immuno-oncology},
  author={Ding, Jiayuan and Venegas, Julian and Lu, Qiaolin and Wang, Yixin and Wu, Lidan and Jin, Wei and Wen, Hongzhi and Liu, Renming and Tang, Wenzhuo and Li, Zhaoheng and others},
  journal={bioRxiv},
  pages={2023--04},
  year={2023},
  publisher={Cold Spring Harbor Laboratory}
}
}
```
