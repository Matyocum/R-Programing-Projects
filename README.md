# R-Churn
Customer churn with time series R data 

#### Import data

Telco_Customers <- read_excel("Downloads/Telco_Customers.xlsx")

#### Convert from string to Factor and Numeric variables.

Telco_Customers[,-c(6,19,20)] <- as.data.frame(unclass(Telco_Customers
                [,-c(6,19,20)]),stringsAsFactors = TRUE)

#### Create Barplot for churn data

barplot(table(Telco_Customers$Churn),main = "Churn",col=c("grey","lightblue"),ylim = c(0,6000))

![image](https://user-images.githubusercontent.com/114650133/199350073-f18128d4-4d8f-460f-93e0-33130ff75d63.png)



                
                

















