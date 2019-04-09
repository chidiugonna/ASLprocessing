# ASLprocessing
General Notes on ASL processing

---


### References

|Paper | Description |
|-|-|
|[Alsop et al 2015](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4190138/) Recommended Implementation of Arterial Spin Labeled Perfusion MRI for Clinical Applications: A consensus of the ISMRM Perfusion Study Group and the European Consortium for ASL in Dementia |The ASL white paper which provides rationale for optimal ASL protocols for clinical applications and is a good starting point for ASL.|



---
### BASIL
[Read the Docs](https://asl-docs.readthedocs.io/en/latest/oxasl_userguide.html#usage)
[Wiki](https://fsl.fmrib.ox.ac.uk/fsl/fslwiki/BASIL)
[primers](http://www.neuroimagingprimers.org/examples/introduction-to-perfusion-quantification-using-asl/)


### Command Line
run `createFiles.sh` to separate out M0 and PCASL for example `005`
run `runbasil.sh` to complete command line BASIL
gui version can be run with `asl_gui`

#### Comparison of Axial vs Oblique (AC-PC) and Whole Brain vs non-WB
001 = Axial-WB
002 = Axial-Non-WB
003 = Oblique-WB
004 = Oblique-Non-WB

#### BASIL GUI
Screenshots
[input data](./docs/inputdata.png)
[structure](./docs/structure.png)
[calibration](./docs/calibration.png)
[distortion correction](./docs/distortioncorrection.png)
[analysis](./docs/Analysis.png)
[running screen](./docs/run.png)


##### local locations
Non-BS images - `/media/chidi/Pluto/RESEARCH/ASL/NK-acq`
Axial/Oblique vs WB/small-FOV - `/media/chidi/Pluto/RESEARCH/ASL/Ted-acq`
---
### ASLTlbx
download SPM-12 version of ASLtlbx from https://cfn.upenn.edu/~zewang/ASLtbx.php
downloaded as `ASLtbx2.zip` and extracts to `batch_scripts_pcasl`

##### local locations
[custom ASLTlbx](/media/chidi/DATA/RESEARCH/NKLAB/ASL/ASLTlbx/SPM12/ASLtbx2)
[custom perf_reconstruct_SPM8_GRASE.m](/media/chidi/DATA/RESEARCH/NKLAB/ASL/ASLTlbx/SPM12/ASLtbx2)