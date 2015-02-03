## Exploratory Data Analysis First Project

This assignment uses data from the [UC Irvine Machine Learning Repository][1],
a popular repository for machine learning datasets.
In particular, we will be using the _Individual household electric power 
consumption Data Set_ which is available on the course web site:

* __Dataset__: [Electric power consumption][2] [20Mb]

* __Description__: Measurements of electric power consumption in one household
with a one-minute sampling rate over a period of almost 4 years.
Different electrical quantities and some sub-metering values are available.

The following descriptions of the 9 variables in the dataset are taken from the
[UCI web site][3]:

1. __Date__: Date in format dd/mm/yyyy
2. __Time__: time in format hh:mm:ss
3. __Global_active_power__: household global minute-averaged active power
   (in kilowatt)
4. __Global_reactive_power__: household global minute-averaged reactive power
   (in kilowatt)
5. __Voltage__: minute-averaged voltage (in volt)
6. __Global_intensity__: household global minute-averaged current intensity
   (in ampere)
7. __Sub_metering_1__: energy sub-metering No. 1 (in watt-hour of active
   energy).
   It corresponds to the kitchen, containing mainly a dishwasher, an oven and a
   microwave (hot plates are not electric but gas powered)
8. __Sub_metering_2__: energy sub-metering No. 2 (in watt-hour of active energy).
   It corresponds to the laundry room, containing a washing-machine, a
   tumble-drier, a refrigerator and a light
9. __Sub_metering_3__: energy sub-metering No. 3 (in watt-hour of active energy).
   It corresponds to an electric water-heater and an air-conditioner.

## Loading the data

The R script called `getdata.R` provides the function `getdata()` for
downloading the data set and unzipping it in the folder specified by the
parameter `destdir`. Just run:

```r
source( "./getdata.R" )
getdata( destdir = "./data" )
```

[1]: http://archive.ics.uci.edu/ml/
[2]: https://d396qusza40orc.cloudfront.net/exdata%2Fdata%2Fhousehold_power_consumption.zip
[3]: https://archive.ics.uci.edu/ml/datasets/Individual+household+electric+power+consumption