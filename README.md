<img src="Tcell.png" align="left" width="120" heigth="120"/>

# plattner_mcb_2024

&nbsp;
&nbsp;
&nbsp;
&nbsp;

&nbsp;
&nbsp;
&nbsp;
&nbsp;

Jupyternotebook for analysing single-cell TCR repertoires and gene expression from the demo data set "Human TCR/BCR Full Length Demo Data" provided by BD (https://scomix.bd.com/hc/en-us/articles/4424059302157-Rhapsody-TCR-BCR-Full-Length-Demo-Dataset).


## Environment setup and software installation

### Clone the repo

```
git clone https://github.com/icbi-lab/plattner_mcb_2024.git
```

### Obtain the data

```
$ URL='https://bd-rhapsody-public.s3.amazonaws.com/Rhapsody-Demo-Data/VDJ'
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

$ pip install anndata==0.10.8
$ pip install muon==0.1.6
$ pip install numpy==2.0.2
$ pip install pandas==2.2.3
$ pip install scanpy==1.10.3
$ pip install scirpy==0.17.2
$ pip install matplotlib==3.9.4
$ pip install seaborn==0.13.2
$ pip install ipykernel==6.29.5
$ pip install ipywidgets==8.1.5

$ python -m ipykernel install --user --name plattner_mcb_2024 --display-name "plattner_mcb_2024"
```
