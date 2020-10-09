# RAzureInterfaces
Introduction to R interfaces to Azure

Embarrasingly parallel computation with Azure Batch, `foreach` and `doAzureParallel`


## On RMarkdown vs Jupyter Notebook formats

### RMarkdown highlights
\+ Code and output are strictly separated. Thus, source files `.Rmd` are easy to edit and git-friendly. Output files `.nb.html` can be left out of version control altogether.  
\+ High control on the format of code chunks. For example, it is very easy and transparent to configure code chunks to be shown in the output but not evaluated, or the other way around.  
\+ Modularity. Easy to organize large notebooks on modular files.  
\- Code chunks cannot be evaluated on an environment that shows rendered markdown (at least in the popular R IDEs or online notebooks servers)

### Jupyter highlights
\+ Code chunks can be evaluated on an environment with rendered markdown text. Hence the same environment offers good aesthetics and interactive code execution. Ideal for a live presentation.
\+ High control over visibility and user interaction, specially if using extensions.  
\- Source code and output confounded in complex `ipynb` (json) files.
