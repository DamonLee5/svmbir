<<<<<<< HEAD
svmbir
======

* Python code for fast parallel-beam MBIR (Model Based Iterative Reconstruction)

* This is a python wrapper around HPImaging's supervoxel C code, [sv-mbir](https://github.com/HPImaging/sv-mbirct).
=======
**svmbir** stands for Super-Voxel Model-Based Iterative Reconstruction.
svmbir is an easy-to-use python package for fast parallel-beam reconstruction of tomography data using model-based priors.


Features
--------
* Easy-to-use python code for fast parallel-beam MBIR (Model Based Iterative Reconstruction)

* Interface to HPImaging's C code implementation of the super-voxel algorithm :cite:`wang2016high` :cite:`wang2017massively`, `[sv-mbirct] <https://github.com/HPImaging/sv-mbirct>`_

* Supports MBIR reconstruction with Bayesian and Plug-and-Play prior models.

>>>>>>> bd1db18a94c00438eb2f3d35ed483f0bbae8d377

System Requirements
-------------------
1. GCC compiler version 4.8.5 or above
<<<<<<< HEAD
2. OpenMP API
3. Python>=3.6

(Python dependencies are automatically installed upon installation of svmbir)


Optional System Requirements for faster reconstruction
------------------------------------------------------
1. Intel-based CPU(s)
2. Intel ICC compiler (included in "Parallel Studio XE", available from Intel for Linux, macOS)

It is recommended that you install svmbir in a [conda environment](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html).
=======
2. OpenMP Libraries
3. Python>=3.6


Optional System Requirements
----------------------------
Fastest reconstruction can be obtained with,

* Intel-based CPU(s) supporting AVX2,AVX512
* Intel ICC compiler (in "Parallel Studio XE", and now free "oneAPI")

We also recommend:

* Installation using conda environment

License
-------
The project is licensed under the `BSD 3-Clause <https://github.com/cabouman/svmbir/blob/master/LICENSE>`_ License.


>>>>>>> bd1db18a94c00438eb2f3d35ed483f0bbae8d377
