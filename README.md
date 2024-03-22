# plattner_mcb_2024

Jupyternotebook for analysing single-cell TCR repertoires and gene expression from the demo data set "Human TCR/BCR Full Length Demo Data" provided by BD (https://scomix.bd.com/hc/en-us/articles/4424059302157-Rhapsody-TCR-BCR-Full-Length-Demo-Dataset).


## Environment setup and software installation

### Clone the repo

```
git clone https://github.com/icbi-lab/plattner_mcb_2024.git
```

### Obtain the data

```
$ URL='https://bd-rhapsody-public.s3.amazonaws.com/Rhapsody-Demo-Data/VDJ/'
$ DATA_FILE='RhapTCRBCRdemo.zip'
$ cd plattner_mcb_2024
$ mkdir data
$ cd data
$ curl -o $DATA_FILE ${URL}/${DATA_FILE}
$ unzip $DATA_FILE
```

### Setup conda environment

```
$ conda create -n plattner_mcb_2024 python==3.9
$ conda activate plattner_mcb_2024

$ pip install anndata
$ pip install muon
$ pip install numpy
$ pip install pandas
$ pip install scanpy
$ pip install scirpy
$ pip install ipykernel
$ pip install ipywidgets

$ python -m ipykernel install --user --name plattner_mcb_2024 --display-name "plattner_mcb_2024"
```
