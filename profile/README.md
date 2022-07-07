
# OpenNeuro Derivatives
This is a collection of [BIDS](https://bids.neuroimaging.io/) 
[Derivatives](https://bids-specification.readthedocs.io/en/stable/05-derivatives/01-introduction.html) datasets created by running 
[fMRIPrep](https://fmriprep.org/en/stable/) and/or [MRIQC](https://mriqc.readthedocs.io/en/latest/) 
on [OpenNeuro](https://openneuro.org/) datasets. We will steadily make more datasets available as they are completed.

## Downloading
Datasets can be accessed via [DataLad](https://www.datalad.org/) or S3:

#### Download from S3
```aws s3 sync --no-sign-request s3://openneuro-derivatives/mriqc/ds000102-mriqc ds000102-mriqc```

#### Download with DataLad
```datalad install https://github.com/OpenNeuroDerivatives/ds000102-mriqc.git```

## Superdataset
To see a list of all available datasets, please view the derivatives [superdataset](https://github.com/OpenNeuroDerivatives/OpenNeuroDerivatives).
Individual derivatives datasets can also be accessed as subdatasets within the superdataset:
```
datalad install https://github.com/OpenNeuroDerivatives/OpenNeuroDerivatives.git
cd OpenNeuroDerivatives
datalad install ds000102-mriqc
```

## Acknowledgements
These derivatives were generated on the Texas Advanced Computing Center Frontera computing system [1] through their Pathways allocation. 
This work was also funded by the NIH BRAIN Initiative.

[1]: Dan Stanzione, John West, R. Todd Evans, Tommy Minyard, Omar Ghattas, and Dhabaleswar K. Panda. 2020. Frontera: The Evolution of Leadership Computing at the National Science Foundation. In Practice and Experience in Advanced Research Computing (PEARC ’20), July 26–30, 2020, Portland, OR, USA. ACM, New York, NY, USA, 11 pages. https://doi.org/10.1145/3311790.3396656
