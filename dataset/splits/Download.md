\# Dataset Download



This document provides instructions for obtaining the datasets used in the HGD-YOLO experiments.



\## Dataset I



Dataset I contains 15,231 infrared gas leakage images collected from two sources:



\- 3,123 laboratory-acquired ammonia leakage images.

\- 12,108 selected frames from the public IOD-Video dataset.



\### Laboratory-Acquired Dataset



The laboratory-acquired subset contains infrared images of ammonia leakage collected under different leakage rates, thermal contrasts, diffusion patterns, and background conditions.



The laboratory-acquired infrared ammonia leakage dataset and the corresponding YOLO-format annotations are available from the authors upon reasonable request.



\*\*Data request:\*\* Please contact us at 2424420079@ynnu.edu.cn.



\### IOD-Video Dataset



The remaining images in Dataset I were selected from the publicly available IOD-Video dataset.



Please obtain the original IOD-Video dataset from its official source:



**Official dataset access:** The IOD-Video dataset can be obtained by contacting Kailai Zhou at calayzhou@smail.nju.edu.cn or DG21230090@smail.nju.edu.cn. A preview of the dataset is available via NJU Box. Upon request, the dataset authors will provide download links via NJU Box, Baidu Cloud, and Google Drive.



For reproducibility, the exact frame manifests used in our experiments are provided in the `splits/` directory:



\- `Dataset\_I\_train.txt`

\- `Dataset\_I\_val.txt`

\- `Dataset\_I\_test.txt`



\## Dataset II



Dataset II contains 4,983 non-overlapping images selected from the IOD-Video dataset and is used to evaluate the generalization performance of HGD-YOLO.



The experimental split is organized as follows:



\- Training: 3,488 images

\- Validation: 996 images

\- Test: 499 images



The exact frame manifests are provided in the `splits/` directory:



\- `Dataset\_II\_train.txt`

\- `Dataset\_II\_val.txt`

\- `Dataset\_II\_test.txt`



Users should first obtain the original IOD-Video dataset from its official source and then use the provided frame manifests to reconstruct the subsets used in our experiments.



\## Annotation Format



All samples used in this study are organized in YOLO detection format. Each image has a corresponding `.txt` annotation file with the same base filename.



Each annotation is represented as:



`<class\_id> <x\_center> <y\_center> <width> <height>`



where the bounding-box coordinates are normalized with respect to the image width and height.



The experiments in this study involve a single gas-leakage category.



\## Notes



The original IOD-Video data are not redistributed in this repository. Users should obtain the dataset from its official source and comply with the corresponding license and terms of use.



The laboratory-acquired infrared ammonia leakage dataset and its annotations can be obtained from the authors upon reasonable request by contacting 2424420079@ynnu.edu.cn.



The provided split files record the exact samples used in our experiments to facilitate reproducibility.

