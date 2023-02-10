Moving Towards Reproducible and Programmatic Generation of Neuroimaging
Visualizations
================

## Reference

**Chopra, S.**, Labache, L., Dhamala, E., Orchard, E., Holmes. A. [A
Practical Guide for Generating Reproducible and Programmatic
Neuroimaging
Visualizations](https://github.com/sidchop/RepoNeuroVis/blob/main/manuscript.pdf).

------------------------------------------------------------------------

## Background

Neuroimaging visualizations form the centerpiece of the interpretation
and communication of scientific results, and are also a cornerstone for
data quality control. Often, these images and figures are produced by
manually changing settings on Graphical User Interfaces (GUIs). There
now exist many well-documented code-based brain visualization tools that
allow users to programmatically generate publication-ready figures
directly within R, Python and MATLAB environments. Here, we provide a
rationale for the wide-spread adoption of code-generated brain
visualizations by highlighting corresponding advantages in
replicability, flexibility, and integration over GUI based tools. We
then provide a practical guide outlining the steps required to generate
these code-based brain visualizations. We also present a comprehensive
table of tools currently available for programmatic brain visualizations
and provide didactic examples of visualizations and associated code as a
point of reference. Finally, we provide a web-app
(<https://sidchop.shinyapps.io/braincode/>) which can generate simple
code-templates as starting points for these visualizations..

------------------------------------------------------------------------

## Examples of code-based neuroimaging visualizations tools that can be accessed directly within R, MATLAB and Python environments.

|                                                                                                                         | Voxel                        | Vertex                      | ROI                            | Edge                      | Streamlines             |
|:------------------------------------------------------------------------------------------------------------------------|:-----------------------------|:----------------------------|:-------------------------------|:--------------------------|:------------------------|
| **R**                                                                                                                   |                              |                             |                                |                           |                         |
|   [ANTsR](https://antsx.github.io/ANTsR/articles/ANTsR.html)                                                            | ***+<sup>2</sup>***          | ***+<sup>2</sup>***         | ***+<sup>2</sup>***            | ***+<sup>1</sup>***       |                         |
|   [brainconn](https://github.com/sidchop/brainconn)                                                                     |                              |                             |                                | ***+<sup>1</sup>***       |                         |
|   [brainR](https://github.com/muschellij2/brainR)                                                                       | ***+<sup>2,6,7</sup>***      |                             | ***+<sup>6,7</sup>***          |                           |                         |
|   [ciftitools](https://github.com/mandymejia/ciftiTools)<sup>**^**</sup>                                                | ***+<sup>2,3</sup>***        | ***+<sup>2,3</sup>***       | ***+\*<sup>,2,3</sup>***       |                           |                         |
|   [fsbrain](https://github.com/dfsp-spirit/fsbrain)<sup>**^**</sup>                                                     | ***+<sup>4</sup>***          | ***+<sup>3,4</sup>***       | ***+\*<sup>,6,3,4</sup>***     |                           |                         |
|   [ggseg](https://github.com/ggseg/ggseg)<sup>**^**</sup>                                                               |                              |                             | ***+<sup>1,4</sup>***          |                           |                         |
|   [neurobase](https://github.com/muschellij2/neurobase)                                                                 | ***+<sup>2</sup>***          |                             |                                |                           |                         |
|   [oro.nifti](https://github.com/muschellij2/oro.nifti)                                                                 | ***+<sup>2</sup>***          |                             |                                |                           |                         |
| **Python**                                                                                                              |                              |                             |                                |                           |                         |
|   [ANTsPy](https://github.com/ANTsX/ANTsPy)                                                                             | ***+<sup>2</sup>***          | ***+<sup>2</sup>***         | ***+<sup>2</sup>***            |                           |                         |
|   [brainiak](https://github.com/brainiak/brainiak)                                                                      | ***+<sup>2</sup>***          |                             |                                |                           |                         |
|   [Brainplotlib](https://github.com/feilong/brainplotlib)                                                               |                              | ***+<sup>1,11</sup>***      | ***+\*<sup>,1,11</sup>***      |                           |                         |
|   [Brainspace](https://github.com/MICA-MNI/BrainSpace)/[surfplot](https://github.com/danjgale/surfplot)<sup>**^**</sup> |                              | ***+<sup>3,4,6,7.8</sup>*** | ***+\*<sup>,3,4,6,7,8</sup>*** |                           |                         |
|   [DIPY](https://github.com/dipy/dipy)<sup>**^**</sup>                                                                  | ***+<sup>2</sup>***          |                             |                                |                           | ***+<sup>5,9</sup>***   |
|   [ENIGMA TOOLBOX](https://github.com/MICA-MNI/ENIGMA)<sup>**^**</sup>                                                  |                              |                             | ***+<sup>1,3,4,6,8</sup>***    |                           |                         |
|   [FSLeyes](https://github.com/pauldmccarthy/fsleyes)                                                                   | ***+<sup>2,3,4</sup>***      | ***+<sup>2,3,4</sup>***     | ***+<sup>2,3,4</sup>***        |                           | ***+<sup>2,5</sup>***   |
|   [ggseg](https://github.com/ggseg/python-ggseg)                                                                        |                              |                             | ***+<sup>1,4</sup>***          |                           |                         |
|   [graphpype](https://neuropycon.github.io/graphpype/)                                                                  |                              |                             |                                | ***+<sup>1,10,11</sup>*** |                         |
|   [MMVT](https://github.com/pelednoam/mmvt)                                                                             |                              | ***+2,4***                  | ***+2,4***                     | ***+<sup>1,10,11</sup>*** |                         |
|   [MNE](https://github.com/mne-tools/mne-python)                                                                        | ***+<sup>2,4</sup>***        | ***+<sup>4</sup>***         | ***+<sup>4</sup>***            |                           |                         |
|   [mrivis](https://github.com/raamana/mrivis)                                                                           | ***+<sup>2</sup>***          |                             |                                |                           |                         |
|   [NaNSlice](https://github.com/spinicist/nanslice)                                                                     | ***+<sup>2</sup>***          |                             |                                |                           |                         |
|   [netneurotools](https://github.com/netneurolab/netneurotools)                                                         |                              | ***+<sup>4</sup>***         | ***+\*<sup>,3</sup>***         |                           |                         |
|   [netplotbrain](https://github.com/wiheto/netplotbrain)<sup>**^**</sup>                                                |                              |                             | ***+<sup>1,2</sup>***          | ***+<sup>1,11</sup>***    |                         |
|   [nilearn](https://github.com/nilearn/nilearn)<sup>**^**</sup>                                                         | ***+<sup>2</sup>***          | ***+<sup>2,3</sup>***       | ***+<sup>2,3</sup>***          | ***+<sup>1,11</sup>***    |                         |
|   [niwidget](https://github.com/nipy/niwidgets)                                                                         | ***+<sup>2,3,4</sup>***      | ***+<sup>2,3,4</sup>***     |                                |                           | ***+<sup>5</sup>***     |
|   [Pycortex](https://github.com/gallantlab/pycortex)                                                                    | ***+<sup>8,11,12</sup>***    | ***+<sup>4,8,11,12</sup>*** | ***+\*<sup>,4,8,11,12</sup>*** |                           |                         |
|   [pySurfer](https://pysurfer.github.io/)<sup>**^**</sup>                                                               |                              | ***+<sup>4</sup>***         | ***+\*<sup>,4</sup>***         |                           |                         |
|   [surfice](https://github.com/neurolabusc/surf-ice)                                                                    | ***+<sup>2,3,4</sup>***      | ***+<sup>2,3,4</sup>***     | ***+<sup>2,3,4,6</sup>***      | ***+<sup>1,4,6</sup>***   | ***+<sup>4,5,6</sup>*** |
|   [Visbrain](https://github.com/EtienneCmb/visbrain)                                                                    | ***+<sup>1,2,3,6</sup>***    | ***+<sup>1,2,3,6</sup>***   | ***+<sup>1,2,3,6</sup>***      | ***+<sup>1,2,3,6</sup>*** |                         |
| **MATLAB**                                                                                                              |                              |                             |                                |                           |                         |
|   [BrainNetViewer](https://www.nitrc.org/projects/bnv/)                                                                 | ***+<sup>2,3,4,6,13</sup>*** |                             | ***+<sup>2,3,4,6,13</sup>***   | ***+<sup>1,10</sup>***    |                         |
|   [Brainspace](https://github.com/MICA-MNI/BrainSpace)<sup>**^**</sup>                                                  |                              | ***+<sup>3,4,6,7,8</sup>*** | ***+\*<sup>,3,4,6,7,8</sup>*** |                           |                         |
|   [Brainstorm](https://github.com/brainstorm-tools/brainstorm3)                                                         | ***+<sup>2</sup>***          | ***+<sup>4,6</sup>***       | ***+<sup>3,4,6</sup>***        |                           |                         |
|   [bspmview](https://www.bobspunt.com/software/bspmview/)                                                               | ***+<sup>2,13</sup>***       |                             | ***+<sup>2,13</sup>***         |                           |                         |
|   [CandlabCore](https://github.com/canlab/CanlabCore)                                                                   | ***+<sup>2,10,13</sup>***    |                             | ***+<sup>2,10,13</sup>***      |                           |                         |
|   [ECoG/fMRI Vis toolbox](https://github.com/Immiora/matlab-ecog-visualization)                                         |                              | ***+<sup>10</sup>***        | ***+\*<sup>,10</sup>***        |                           |                         |
|   [ENIGMA TOOLBOX](https://github.com/MICA-MNI/ENIGMA)<sup>**^**</sup>                                                  |                              |                             | ***+<sup>1,10</sup>***         |                           |                         |
|   [FieldTrip](https://www.fieldtriptoolbox.org/)                                                                        | ***+<sup>2</sup>***          | ***+<sup>10</sup>***        |                                |                           |                         |
|   [Lead-DBS](https://www.lead-dbs.org/)                                                                                 | ***+<sup>2</sup>***          |                             | ***+<sup>2,3,4</sup>***        |                           |                         |
|   [mni2fs](https://github.com/dprice80/mni2fs)                                                                          |                              | ***+<sup>2,3</sup>***       |                                |                           |                         |
|   [mrtools](https://github.com/justingardner/mrTools)                                                                   | ***+<sup>2</sup>***          | ***+<sup>4,12</sup>***      | ***+\*<sup>,2,4,12</sup>***    |                           |                         |
|   [plotSurfaceROIBoundary](https://github.com/StuartJO/plotSurfaceROIBoundary)                                          |                              | ***+<sup>4,10</sup>***      | ***+\*<sup>,4,10</sup>***      |                           |                         |
|   [Vistasoft](http://web.stanford.edu/group/vista/cgi-bin/wiki/index.php/Visualization)                                 | ***+<sup>2</sup>***          | ***+<sup>2</sup>***         | ***+<sup>2</sup>***            |                           | ***+<sup>10</sup>***    |

Note: The tools listed contain functionality required to generate (at
least close-to) publication-ready neuroimaging figures via user-entered
code within R, MATLAB and Python environments. This list does not
include cross-platform general purpose visualization software. **1** =
.txt/.csv (scalar, vector, matrix as input); **2** = .nii/.nii.gz (nifti
as input); **3** = .cii/.gii (cifti or gifti files as input, includes
any subtypes e.g. dlabel, dtseries, .surf); **4** = FreeSurfer formats
as input, including .mgz, .annot, .label, .curv, .wm etc); **5** =
.trk/.tck (tractograms as input); **6** = .obj (3D object format); **7**
= .ply (3D polygon format); **8** = .vtk (Visualization Toolkit format);
**9** = .fib (Legacy vtk format); **10** = .mat (MATLAB format); 11 =
.npy/.npz (Python numpy format); **12** = .off (object file format);
***\**** = Cortex only; **^** = Well-documented, beginner friendly
code-based visualization tool (note that this is a subjective criteria
intended to guide new-users, and many other tools in this table may also
meet this criteria).

|                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Brain-Code: A web-app for generating code templates for brain visualizations                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| To assist new users transition into generating code-based brain visualizations we have developed a web-app (<https://sidchop.shinyapps.io/braincode/>) which allows for interactive generation of code-templates for beginner friendly libraries/packages in R and Python. In the web-app, users can select R or Python as their coding environment, and choose between voxel, ROI, vertex, and edge-level visualizations. They can then manually adjust a limited set of visualization setting, such as color-scales and view, and are provided with a reactive code-template which can be copied and then used within their respective programming environment. The provided code templates require users to customize the code, such as alter file-paths. The available settings have been purposefully limited to allow users to explore and fine-tune additional visualization options within their own programming environment. The code-template also contains links and prompts to more detailed documentation, alternate packages/libraries and tutorials which allow for more complex and publication-ready brain visualizations. |
|                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| <img src="images/image-17223477.png" width="100%" height="70%" style="display: block; margin: auto;" />                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |

## Examples of figures made in R:  

<img src="data/readme_figures/fig1.png" width="50%" />

## Examples of figures made in Python: 

<img src="data/readme_figures/fig2.png" width="50%" />

## Questions

Please contact me (Sidhant Chopra) as <sidhant.chopra@yale.edu> and/or
<sidhant.chopra4@gmail.com>
