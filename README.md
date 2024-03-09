# SMART Dashboard Installation

## Step 1: Download Files

   Download all files from this repository to your local machine. The easiest way to accomplish this is by navigating to the desired directory and using the `git clone` command.

   If on Windows, open Powershell; if on Mac, open Terminal. You will be met with a command prompt displaying your current working directory: 

   ```
   PS:\Users\ntedesco>
   ```

   Next, navigate to your desired location. For example, I would like to download all files in this repo to my `Projects` folder within `Documents`. *NOTE: Cloning the repo will automatically create a folder for all downloaded files, so no need to manually create a `dashboard` folder.*

   ```
   cd Documents\dashboard
   ```

   Finally, download all files from this repo into the target destination: 

   ```
   git clone https://github.com/ntedesco-umich/SMART-dashboard/
   ```

## Step 2: Install Packages 

   Docker is the most efficient way to share applications without worrying about local package conflicts. However, the process of setting up a Docker container is a bit involved, so we'll start by trying to manually install the necessary R packages. 

   Open RStudio and run the following commands in the console: 

   ```
   install.packages(c('devtools', 'tidyverse', 'flexdashboard', 'knitr', 'plotly', 'shiny', 'RColorBrewer', 'stringr', 'shinymanager', 'shinythemes', 'shinyTime', 'DT', 'highcharter', 'readr', 'lubridate', 'httr', 'blockrand'), dependencies = TRUE, repo='http://cran.r-project.org')

   devtools::install_github("davidsjoberg/ggsankey")
   ```

   This will take a moment to complete. Let me know if you are still missing any packages after attempting Step 3. 

## Step 3: Run the Dashboard

   Open flexdashboard.Rmd and click `Run Document` at the top of the page. You should be good to go! 

