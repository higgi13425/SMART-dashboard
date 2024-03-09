# SMART Dashboard Installation

## Step 1: Download Files

   Download all files from repository to local machine. The easiest way to accomplish this is by navigating to the desired location, and using the `git clone` command to clone the repository.

   If on Windows, open Powershell; if on Mac, open Terminal. You will be met with a command prompt displaying your current working directory: 

   `PS:\Users\ntedesco>`

   Next, navigate to your desired location. I would like to install the files within the `dashboard` subfolder of my `Documents` folder. 

   `PS:\Users\ntedesco> cd Documents\dashboard`

   Finally, download all files from this repository into the target destination: 

   `PS:\Users\ntedesco\Documents\dashboard> git clone https://github.com/ntedesco-umich/SMART-dashboard/`

## Step 2: Install Packages 

   The most efficient way to share applications across different machines without having to worry about package conflicts is to use a Docker container. However, this process is a bit involved, so let's just try manually installing the R packages necessary for the dashboard. 

   Open R and run the following command: 

   `install.packages(c("))

   When you attempt to run the dashboard, it will throw an error mentioning any missing packages - let me know if this happens to you. 

## Step 3: Run the Dashboard

   

