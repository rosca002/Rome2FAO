# Rome2FAO

## Install necessary packages

    install.packages("MASS")
    install.packages("ggplot2")
    install.packages("reshape2")

## Downloading the data ####

    workshop_folder <- "~/wur_Rome2FAO" 
    if(!file.exists(file.path(workshop_folder,"data.zip"))){
      download.file("https://www.dropbox.com/sh/ve7dck9aj2jj180/AABvPXMZ72CqpQN8s1tmOhm2a?dl=1",
                    file.path(workshop_folder,"data.zip"),"auto",mode="wb")
      unzip(file.path(workshop_folder,"data.zip"),exdir=file.path(workshop_folder,"data"))
    }
