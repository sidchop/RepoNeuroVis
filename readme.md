A Practical Guide for Generating Reproducible and Programmatic
Neuroimaging Visualizations
================

## Paper

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
(<https://sidchop.shinyapps.io/braincode_selector/>) and provide
didactic examples of visualizations and associated code as a point of
reference. Finally, we provide a web-app
(<https://sidchop.shinyapps.io/braincode/>) which can generate simple
code-templates as starting points for these visualizations.

**Full paper:** [A Practical Guide for Generating Reproducible and
Programmatic Neuroimaging
Visualizations](https://github.com/sidchop/RepoNeuroVis/blob/main/manuscript.pdf).
Chopra, Sidhant., Labache, L., Dhamala, E., Orchard, E., Holmes. A.

------------------------------------------------------------------------

## Tool finder:

To assists researchers in finding a code-based brain visualization tool,
we have provided a interactive table:
<https://sidchop.shinyapps.io/braincode_selector/>. If you think that we
have missed a code-based package/library or tool box which can generate
brain visualization directly witin in R, python or MATLAB environments,
please [creating an issue on this GitHub
page](https://github.com/sidchop/RepoNeuroVis/issues) or leave a comment
on this [google
sheet](https://docs.google.com/spreadsheets/d/1vTqeTSV1K4SfeH7KWtSDPHKJMhNsRcB3W3rYNRdxQKc/edit#gid=0).

------------------------------------------------------------------------

## Template generator (R & Python):

[Brain-Code: A web-app for generating code templates for brain
visualizations](https://sidchop.shinyapps.io/braincode/)

To assist new users transition into generating code-based brain
visualizations we have developed a web-app
(<https://sidchop.shinyapps.io/braincode/>) which allows for interactive
generation of code-templates for beginner friendly libraries/packages in
R and Python. In the web-app, users can select R or Python as their
coding environment, and choose between voxel, ROI, vertex, and
edge-level visualizations. They can then manually adjust a limited set
of visualization setting, such as color-scales and view, and are
provided with a reactive code-template which can be copied and then used
within their respective programming environment. The provided code
templates require users to customize the code, such as alter file-paths.
The available settings have been purposefully limited to allow users to
explore and fine-tune additional visualization options within their own
programming environment. The code-template also contains links and
prompts to more detailed documentation, alternate packages/libraries and
tutorials which allow for more complex and publication-ready brain
visualizations. **Note:** This web-app is still under development, so
some features are a little slow and we are working on the UI. Please
feel free to leave feedback by [creating an issue on this GitHub
page](https://github.com/sidchop/RepoNeuroVis/issues).

## <img src="images/image-17223477.png" width="100%" height="70%" style="display: block; margin: auto;" />

## Examples of figures made within R and Python:  

<img src="data/readme_figures/fig1.png" width="70%" style="display: block; margin: auto;" />

## Examples of figures made in Python: 

<img src="data/readme_figures/fig2.png" width="70%" style="display: block; margin: auto;" />

## Questions

Please contact me (Sidhant Chopra) as <sidhant.chopra@yale.edu> and/or
<sidhant.chopra4@gmail.com>
