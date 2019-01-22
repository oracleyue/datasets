# Folder Descriptions


## Test Datasets

The data sets are simulation of dynet in the form of ARX.  Here are two cases: one
with different SNRs (i.e. `SNR`); the other with different #nodes (i.e. `p`).

`dataARX_snr`:  simulation with different SNRs (SNR = 0, 10, 20, 40 dB) and p = 10.  
`dataARX_p`: simulation with different #nodes (p = 5, 10, 15, 20) and SNR = 10 dB.

## Test 1

This test uses groupSBL to run network inference on 50 datasets. 

`resARX_gsbl_p`: the multiple tests with 50 datasets, 10 nodes (p = 10, m = 1); using groupSBL with 1e-3 for PruneGamma.

`resARX_gsbl_snr`: the multiple tests with 50 datasets, SNR = 10 dB; using groupSBL with 1e-3 for PruneGamma.

List of included folders:

-  `dataARX_p`
-  `dataARX_snr`
-  `resARX_gsbl_p`
-  `resARX_gsbl_snr`
    
## Test 2

This test uses group Iterative Reweighted L1 method to run network inference on 50 datasets, which are the same datasets used in Test 1.

`resARX_gil1_p`: the multiple tests with 50 datasets, 10 nodes (p = 10, m = 1) using groupIRL1; The different lambdas (regularization parameters) for p=5, 10, 15, 20 are lambda = 5e-2, 1e-1, 1e-1, 1e-1.

`resARX_gil1_snr`: the multiple tests with 50 datasets, SNR = 10 dB using groupIRL1. The different lambdas (regularization parameters) for SNR=0, 10, 20, 40 are lambda = 1e-1, 1e-1, 1e-2, 1e-3.

List of included folders:

-  `dataARX_p`
-  `dataARX_snr`
-  `resARX_gil1_p`
-  `resARX_gil1_snr`
