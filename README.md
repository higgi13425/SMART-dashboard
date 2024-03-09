# SMART Dashboard Installation

## Step 1: Download Files

   Download all files from repository to local machine. The easiest way to accomplish this is by navigating to the desired location, and using the `git clone` command to clone the repository.

   If on Windows, open Powershell; if on Mac, open Terminal. You will be met with a command prompt displaying your current working directory: 

   ```
   PS:\Users\ntedesco>
   ```

   Next, navigate to your desired location. For example, I would like to download all files in the repository to my `Projects` folder within `Documents`. *NOTE: Cloning the repo will automatically create a folder for all downloaded files, so no need to manually create a `dashboard` folder.*

   ```
   cd Documents\dashboard
   ```

   Finally, download all files from this repository into the target destination: 

   ```
   git clone https://github.com/ntedesco-umich/SMART-dashboard/
   ```

## Step 2: Install Packages 

   The most efficient way to share applications across different machines without having to worry about package conflicts is to use a Docker container. However, this process is a bit involved, so let's just try manually installing the R packages necessary for the dashboard. 

   Open RStudio and run the following commands in the console: 

   ```
   install.packages(c('devtools', 'tidyverse', 'flexdashboard', 'knitr', 'plotly', 'shiny', 'RColorBrewer', 'stringr', 'shinymanager', 'shinythemes', 'shinyTime', 'DT', 'highcharter', 'readr', 'lubridate', 'httr', 'blockrand'), dependencies = TRUE, repo='http://cran.r-project.org')

   devtools::install_github("davidsjoberg/ggsankey")
   ```

## Step 3: Run the Dashboard

   Open flexdashboard.Rmd and click `Run Document` at the top of the page. You should be good to go! 

