# Build and Test

**Project:** `LUSTRE`
**Upstream:** https://github.com/nicedoc/lustre
**License:** GPL/MIT

## Quick Start

```bash
git clone https://github.com/nicedoc/lustre
cd lustre
pip install -r requirements-anticloud.txt
python anticloud_main.py --offline --pax-local
```

## Anticloud Improvements Applied

1. PAX L5 Narrow L2 General 27B local job scheduling and resource optimization
2. AIOSS tamper-evident HPC job audit chain (cost and energy tracking)
3. AES-256 encryption for all job scripts and output data
4. Single-binary HPC management tool replacing vendor-locked scheduler add-ons
5. Zero-cloud: all monitoring and orchestration runs on head nodes
6. GPU/CPU equalizer: workload profiling adapts to GPU/CPU mix dynamically
7. Open MPI/SLURM integration replacing proprietary job scheduler interfaces
8. Offline power draw and CO2 dashboard replacing cloud monitoring services

## Benchmark Targets

| Metric | Target |
| --- | --- |
| Latency | Primary inference task: <5s on CPU, <1s on GPU |
| Throughput | Batch processing: >100 items/hour on single CPU server |
| Memory | <8GB RAM for standard deployment |
| Accuracy | Task-specific accuracy within 5% of cloud-API baseline |

## Build Status

Not yet measured. Run verified build and record actual figures above.
