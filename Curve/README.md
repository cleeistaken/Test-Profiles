# Curve
Example of curve testing. Max determined in the first run then used to adjust the iops_rate in other test files.

## Max
```
=============================
JOB_NAME      = job0
VMs           = 16
IOPS          = 26833.38 IO/S
THROUGHPUT    = 107.00 MB/s
R_LATENCY     = 0.00 ms
W_LATENCY     = 11.28 ms
95%tile_R_LAT = 0.00 ms
95%tile_W_LAT = 42.00 ms
=============================
```
27,000 IOPS / (16VM * 4 disks) = ~425 IOPS per disk


## 20% of Max
```
=============================
JOB_NAME      = job0
VMs           = 16
IOPS          = 5440.17 IO/S
THROUGHPUT    = 21.00 MB/s
R_LATENCY     = 0.00 ms
W_LATENCY     = 0.71 ms
95%tile_R_LAT = 0.00 ms
95%tile_W_LAT = 1.00 ms
=============================
```
425 IOPS x 0.2 = 85 IOPS_RATE

## 40% of Max
```
=============================
JOB_NAME      = job0
VMs           = 16
IOPS          = 10880.09 IO/S
THROUGHPUT    = 43.00 MB/s
R_LATENCY     = 0.00 ms
W_LATENCY     = 1.37 ms
95%tile_R_LAT = 0.00 ms
95%tile_W_LAT = 2.00 ms
=============================
```
425 IOPS x 0.4 = 170 IOPS_RATE

### 60% of Max
```
=============================
JOB_NAME      = job0
VMs           = 16
IOPS          = 16320.02 IO/S
THROUGHPUT    = 65.00 MB/s
R_LATENCY     = 0.00 ms
W_LATENCY     = 1.59 ms
95%tile_R_LAT = 0.00 ms
95%tile_W_LAT = 2.00 ms
=============================
```
425 IOPS x 0.6 = 255 IOPS_RATE

### 80% of Max
```
=============================
JOB_NAME      = job0
VMs           = 16
IOPS          = 21759.68 IO/S
THROUGHPUT    = 87.00 MB/s
R_LATENCY     = 0.00 ms
W_LATENCY     = 1.96 ms
95%tile_R_LAT = 0.00 ms
95%tile_W_LAT = 3.00 ms
=============================
```
425 IOPS x 0.8 = 340 IOPS_RATE

### 90% of Max
```
=============================

=============================
```
425 IOPS x 0.9 = 382 IOPS_RATE

### 95% of Max
```
=============================

=============================
```
425 IOPS x 0.95 = 403 IOPS_RATE
