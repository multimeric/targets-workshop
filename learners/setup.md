---
title: Setup
---

## Running on OnDemand

1. Go to https://ondemand.hpc.wehi.edu.au
2. Click RStudio Latest
3. Use the `regular` partition
4. Use `4.2.3` as the R version
5. In the "Additional Modules" box, add `quarto/1.1.189 pandoc/2.3.1 cmake/3.25.1`
6. Set the "Runtime hours" to 5
7. Set the CPUs to 4
8. Set the memory to 10 GB
9. In the console, paste in the following command to install the package dependencies:

```r
install.packages(
  c(
    "conflicted",
    "palmerpenguins",
    "quarto",
    "tarchetypes",
    "targets",
    "tidyverse",
    "visNetwork",
    "crew",
    "crew.cluster"
  )
)
```

Your submission page should look like this:

![](fig/rstudio-ood.png)

::: callout
# Installation Problems?
Make sure Global Options → Python → "Automatically activate project-local Python environments" is unchecked!
![](fig/python-envs.png)
:::
