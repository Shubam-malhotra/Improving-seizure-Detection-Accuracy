#Improving Seizure Detection Using EEG Signals

##Epilepsy
    Epilepsy is a neurological disorder marked by recurrent seizures caused by abnormal electrical activity in the brain. Seizures can range from brief periods of confusion or unconsciousness to convulsions. Causes may include genetics, brain injury, or unknown factors. Treatment typically involves medications, but in some cases, surgery or lifestyle changes are necessary. While epilepsy cannot be cured, it can often be managed effectively.

##Seizure 
    A seizure is a sudden, uncontrolled burst of electrical activity in the brain that can cause changes in behavior, movements, feelings, or consciousness. It can last from a few seconds to a few minutes. Seizures vary in intensity; some might involve staring spells or muscle twitches, while others can lead to convulsions or loss of awareness. Seizures can happen to anyone but are more common in people with epilepsy.

##Epilepsy Seizure Detection
    Epilepsy seizure detection using EEG signals and machine learning involves analyzing brain wave data to identify abnormal patterns that signal a seizure. EEG captures electrical activity in the brain, and during a seizure, this activity shows distinct irregularities. Machine learning algorithms are trained to recognize these patterns from EEG data, enabling automatic and real-time detection of seizures. By applying ML models, it becomes possible to detect seizures more quickly and accurately without the need for constant human monitoring, improving patient care and seizure management for individuals with epilepsy.


#Dataset

##Data set link : https://archive.ics.uci.edu/ml/datasets/Epileptic+Seizure+Recognition
The original EEG dataset consists of recordings from 500 individuals, with each person’s brain activity captured for 23.6 seconds. This time-series data is sampled into 4097 data points per recording, with each data point representing the EEG value at a specific time. The dataset is organized into 5 folders, each containing 100 files, representing different conditions.

To process the data, each set of 4097 data points was divided and shuffled into 23 chunks, each chunk representing 1 second of brain activity with 178 data points. This results in a total of 11,500 rows, where each row consists of 178 features (EEG data points) and a label in column 179 representing the class. The label, y, can take one of five values:

5: EEG recorded with eyes open.
4: EEG recorded with eyes closed.
3: EEG recorded from a healthy brain region.
2: EEG recorded from the tumor-affected region.
1: Recording of seizure activity.

Importantly, only class 1 represents subjects experiencing epileptic seizures, while classes 2, 3, 4, and 5 represent non-seizure conditions. While the dataset has five classes, most researchers focus on binary classification: distinguishing seizure activity (class 1) from non-seizure conditions (classes 2-5). This version of the dataset was created as a .csv file for easier access and processing.
