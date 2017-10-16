
> dat <- read.csv(file='data_merged_all_cleaned.csv', header=TRUE)
> names(dat)
> dat$date <- as.POSIXct(strptime(dat$date, format = "%d/%m/%Y %H:%M", tz="GMT"))
> polarPlot(dat, pollutant='pm10', type='season')

> pdf("filename.pdf")
> // PLOTTING
> dev.off()
