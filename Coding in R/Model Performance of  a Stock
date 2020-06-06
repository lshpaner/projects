#this example uses AAPL ticker symbol as a model
#install.packages("quantmod")
library(quantmod)
close<-c()
returns<-c()
begin_date <- " " # date in YYYY-MM-DD format
end_date <- " " # date in YYYY-MM-DD format
getSymbols("AAPL",from = begin_date, to = end_date, auto.assign = TRUE)
head(AAPL)
close<-AAPL$AAPL.Close
head(close)
returns <- (close/lag(close) - 1)
head(returns)
returns<-returns[-1]
mu<-mean(returns)
mu
s<-sd(returns)
s
