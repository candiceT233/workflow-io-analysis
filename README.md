# workflow-io-analysis


# 1000 Genome
Workflow executable is publicly available here: https://github.com/pegasus-isi/1000genome-workflow/tree/master/bin
Initial sets of input data is publicly available here: https://github.com/pegasus-isi/1000genome-workflow/tree/master/data

Download data workflow and data for execution.


Workflow execution slurm script is provided:
```bash
deception_pfs_1kgenome_parallel_6000_1.sbatch
```

# Workflow I/O Characterization
We uses a version of the Datalife monitoring tool.
A version that outputs json file is located here: https://anonymous.4open.science/r/datalife-E5DF

Download and build Datalife monitoring tool
```
git clone https://anonymous.4open.science/r/datalife-E5D datalife
cd datalife
mkdir build
cd build
ccmake ..
make 
```

# Workflow I/O Analysis
1. A script that collects and arranges all I/O statistics into producer-consumer relationships
```
wf_analysis.ipynb
```

2. A script that generates the analysis graph
```
wf2_IO_3d2d_analysis_1000_genome.ipynb
```

One provided workflow profiling statistics generated from datalife is located under `par_6000_10n_PFS_ps300`.

