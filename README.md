This is the Multi-Axis Temporal RElations for Start-points (i.e., `MATRES`) dataset, collected using the annotation scheme proposed in 

```
@inproceedings{NingWuRo18,
    author = {Qiang Ning and Hao Wu and Dan Roth},
    title = {A Multi-Axis Annotation Scheme for Event Temporal Relations},
    booktitle = {ACL},
    month = {7},
    year = {2018},
    publisher = {Association for Computational Linguistics},
    url = "http://cogcomp.org/papers/NingWuRo18.pdf",
    funding = {AI2, IBM-ILLINOIS C3SR, DEFT, ARL},
}
```
Note in the paper above, we only annotated 36 documents from TimeBank-Dense. But later we have extended to the entire TempEval3 datasets.

The dataset is split into three parts, according to the TempEval3 workshop. That is, TimeBank, AQUAINT, and Platinum. All parts are formatted in the following way:
```
docid, verb1, verb2, eiid1, eiid2, relation
```
A few remarks here:
- The `eiid`s are the same with those in TempEval3
- MATRES is only for verb events, so those nominal events in the original TempEval3 won't appear in MATRES.
- In this repo, we only include those events that are on the main-axis. Please refer to the paper for the definition of main-axis.