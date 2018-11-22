# Rome2FAO

## Install necessary packages

    install.packages(c("MASS","ggplot2","reshape2","randomForest","raster"))

## Download the data ####

    workshop_folder <- "~"
    if(!file.exists(file.path(workshop_folder,"wur_Rome2FAO.zip"))){
       download.file("https://www.dropbox.com/sh/ve7dck9aj2jj180/AABvPXMZ72CqpQN8s1tmOhm2a?dl=1",
                     file.path(workshop_folder,"wur_Rome2FAO.zip"),"auto",mode="wb")
      unzip(file.path(workshop_folder,"wur_Rome2FAO.zip"),exdir=file.path(workshop_folder,"wur_Rome2FAO"))
    }

Go to RStudio and open

    "~/wur_Rome2FAO/forestChangeModels.R"
or

    "~/wur_Rome2FAO/Peru_small_scale_disturbances2.R"
