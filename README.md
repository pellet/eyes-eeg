# AlgoLYNXathon Team A repo

Details of the hackathon can be found [here](https://phas3.notion.site/AlgoLYNXathon-Documents-cceb7f5b7acb4e6e9412640075faadde)

The repo contain three notebooks

1. `eyes-eeg.ipynb` which details how data can be downloaded from Open Neuro page
2. `arshy_preparedata_final.ipynb` which details how `Team A` preprocessed the data to be used in classification
3. `arshy_approach2_2labelclassification.ipynb` which goes through how Team built a `eyes open` / `eyes closed` classification using `Random Forest Classifier`

**Preprocessing Approaches**

The different preproces we used 
- `filter` to filter the signals between desired Hz
- `resample` to resample the eeg signal from acqusition frequency to a desired frequency
- `ICA` to remove `ecg, eog` related artifacts 
- `fized length epochs` to break the continuous signal to number of samples

The following approaches were used to preproces that data
*Approach 1*
- filter between 1 and 40
- resample from 500hz to 100 hz
- remove artifacts based on ICA
- epoch 50s

*Approach 2*
- filter between 1 and 40
- resample from 500hz to 100 hz
- remove artifacts based on ICA
- epoch 50s and average

*Approach 3*
- filter between 1 and 20
- resample from 500hz to 100 hz
- remove artifacts based on ICA on epochs
- epoch 50s

*Approach 4*
- filter between 1 and 20
- resample from 500hz to 100 hz
- remove artifacts based on ICA on epochs
- epoch 50s and average

