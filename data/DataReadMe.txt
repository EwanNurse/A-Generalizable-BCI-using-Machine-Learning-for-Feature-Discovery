Data for each Participant is named:
EEG_Participant(*)_dd_mm_yyyy.mat
Where dd_mm_yyyy is the date EEG recording was made

Each .mat file contains 2 vectors:

1. data_epochs:
The EEG time-series segments are dimension
A x B
where B = number of epochs

and A = N * M
for N = number of channels
and M = number of samples per window

The data is ordered by time then channels i.e. each epoch
is [Ch1_1 .... Ch1_M] ... [ChN_1 ... ChN_M]

2. data_key:
The target class of each epoch
dimension is 1 X B

1 = no-movement class
2 = left hand-squeeze
3 = right hand-squeeze
