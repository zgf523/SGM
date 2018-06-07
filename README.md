# Sequence Generation Model with Global Embedding
This is the code for our paper *SGM: Sequence Generation Model for Multi-label Classification*

***********************************************************

## Datasets
* RCV1-V2
* AAPD

Two dataset are available at https://drive.google.com/file/d/1DbYWVXt_J_6wAgjzVh9LG_MG1UCjBQuS/view?usp=sharing

## Requirements
* Ubuntu 16.0.4
* Python 3.5
* Pytorch 0.3.1

## Reproducibility

## Preprocessing
```
python3 preprocess.py -load_data path_to_data -save_data path_to_store_data 
```
Remember to put the data into a folder and name them *train.src*, *train.tgt*, *valid.src*, *valid.tgt*, *test.src* and *test.tgt*, and make a new folder inside called *data*

***************************************************************

## Training
```
python3 train.py -log log_name -config config_yaml -gpus id
```

****************************************************************

## Evaluation
```
python3 train.py -log log_name -config config_yaml -gpus id -restore checkpoint -mode eval
```

*******************************************************************

## Citation
If you use the above codes or the AAPD dataset we built for your research, please cite the paper:

```
@inproceedings{YangCOLING2018,
   author = {Pengcheng Yang and Xu Sun and Wei Li and Shuming Ma and Wei Wu and Houfeng Wang},
   title = {SGM: Sequence Generation Model for Multi-label Classification},
   booktitle = {{COLING} 2018},
   year = {2018}
}
```
