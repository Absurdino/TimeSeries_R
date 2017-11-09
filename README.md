# TimeSeries_R
R and Time Series analysis

# Let's train Time Series with R
# First, let's see if we can download some data for currencies
# We need to come back to this data thing.. Let's rehearse first

# let's install xts and zoo
install.packages("xts")
library(zoo)

prices <- c(132,45, 130.85, 130.00, 129.55, 130.85)
dates <- as.Date(c("2010-01-04", "2010-01-05", "2010-01-06",
                     "2010-01-07", "2010-01-08"))
ibm.daily <- zoo(prices, dates)
ibm.daily
