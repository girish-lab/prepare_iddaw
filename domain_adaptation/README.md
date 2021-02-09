# AutoNUE2021_domain_adaptation

This repository contains the datasets for Domain Adaptation challenge for AutoNEU 2021, CVPR Workshop. For more details, please visit https://cvit.iiit.ac.in/autonue2021/challenge.html


# Source datasets:
For the Cityscapes dataset, participants are requested to use the fine images (~3200 training samples). Refer: https://www.cityscapes-dataset.com/examples/#fine-annotations. For the other datasets (BDD, GTA and Mapillary), the list of image names are given in the csv files in the folder "Source".

Participants are requested to download the datasets from original websites, given below for easy reference:-
1. https://www.mapillary.com/dataset/vistas?pKey=q0GhQpk20wJm1ba1mfwJmw
2. https://bdd-data.berkeley.edu/ (you might have to click on Advanced tab, and then click on "proceed to bdd-data.berkeley.edu")
3. https://download.visinf.tu-darmstadt.de/data/from_games/

After downloading all the source datasets, move them to folder ./domain_adaptation/source/datasets/ and **run the following commands from public-code**:

```
pip3 install requirements.txt
chmod +x domain_adaptation/source/prep_all.sh
./domain_adaptation/source/prep_all.sh
```

This will create a folder "domain_adaptation/source/source_datasets_dir/" where you will find the images and annotations for the source dataset to be used for this competetion.