# R-Churn
Telecommunications company data with a churn varaibale. Applying the churn data to the other variables to create actionable and insightful visable data.

#### Import data

Telco_Customers <- read_excel("Downloads/Telco_Customers.xlsx")

#### Convert from string to Factor and Numeric variables.

Telco_Customers[,-c(6,19,20)] <- as.data.frame(unclass(Telco_Customers
                [,-c(6,19,20)]),stringsAsFactors = TRUE)

#### Create Barplot for churn data

barplot(table(Telco_Customers$Churn),main = "Churn",col=c("grey","lightblue"),ylim = c(0,6000))

![image](https://user-images.githubusercontent.com/114650133/199350073-f18128d4-4d8f-460f-93e0-33130ff75d63.png)

table(Telco_Customers$Churn,Telco_Customers$gender)
table1<-table(Telco_Customers$Churn,Telco_Customers$gender)
barplot(table1,beside = TRUE, main = "Churn - Gender", ylim = c(0,3000),
        legend.text = row.names(table1),
        col=c("grey","lightblue"),args.legend = list(x="topright"))

![image](https://user-images.githubusercontent.com/114650133/199351017-47beec2a-8e95-4b84-bac2-5529ea604f77.png)

table(Telco_Customers$Churn,Telco_Customers$SeniorCitizen)
table2<-table(Telco_Customers$Churn,Telco_Customers$SeniorCitizen)
barplot(table2,beside = TRUE, main = "Churn - Senior Citizen", ylim = c(0,5000),
        col=c("grey","lightblue"), names=c("Under 65","Over 65"),
        args.legend = list(x="topright"))

![image](https://user-images.githubusercontent.com/114650133/199351145-5e8863de-82fe-484a-a767-228debe89368.png)

table(Telco_Customers$Churn,Telco_Customers$Partner)
table3<-table(Telco_Customers$Churn,Telco_Customers$Partner)
barplot(table3,beside = TRUE, main = "Churn - Partner", ylim = c(0,3000),
        legend.text = row.names(table3),
        col=c("grey","lightblue"),args.legend = list(x="topright"))               
              
![image](https://user-images.githubusercontent.com/114650133/199351371-0442e006-cd8c-4320-97ec-931005cce59b.png)

table(Telco_Customers$Churn,Telco_Customers$Dependents)
table4<-table(Telco_Customers$Churn,Telco_Customers$Dependents)
barplot(table4,beside = TRUE, main = "Churn - Dependents", ylim = c(0,4000),
        legend.text = row.names(table4),
        col=c("grey","lightblue"),args.legend = list(x="topright"))

![image](https://user-images.githubusercontent.com/114650133/199351485-c6a24935-fbb5-4b2f-a6be-53075256be35.png)

table(Telco_Customers$Churn,Telco_Customers$PhoneService)
table5<-table(Telco_Customers$Churn,Telco_Customers$PhoneService)
barplot(table5,beside = TRUE, main = "Churn - Phone Service", ylim = c(0,5500),
        legend.text = row.names(table5),
        col=c("grey","lightblue"),args.legend = list(x="topright"))

![image](https://user-images.githubusercontent.com/114650133/199351564-60e60a40-8672-49d3-98f6-31b7a790e6e5.png)

table(Telco_Customers$Churn,Telco_Customers$MultipleLines)
table6<-table(Telco_Customers$Churn,Telco_Customers$MultipleLines)
barplot(table6,beside = TRUE, main = "Churn - Multiple Lines", ylim = c(0,3500),
        legend.text = row.names(table6),
        col=c("grey","lightblue"),args.legend = list(x="topright"))

![image](https://user-images.githubusercontent.com/114650133/199351655-4a35446c-68c8-42ce-b3cf-045ede4cb47d.png)

table(Telco_Customers$Churn,Telco_Customers$InternetService)
table7<-table(Telco_Customers$Churn,Telco_Customers$InternetService)
barplot(table7,beside = TRUE, main = "Churn - Internet Service", ylim = c(0,2500),
        legend.text = row.names(table7),
        col=c("grey","lightblue"),args.legend = list(x="topright"))

![image](https://user-images.githubusercontent.com/114650133/199351744-3416e406-a3d0-4812-819c-59f1d487aacc.png)

table(Telco_Customers$Churn,Telco_Customers$OnlineSecurity)
table8<-table(Telco_Customers$Churn,Telco_Customers$OnlineSecurity)
barplot(table8,beside = TRUE, main = "Churn - Online Security", ylim = c(0,2500),
        legend.text = row.names(table8),
        col=c("grey","lightblue"),args.legend = list(x="topright"))

![image](https://user-images.githubusercontent.com/114650133/199351823-d46f1a89-138f-4c40-a399-183dca4ee802.png)

table(Telco_Customers$Churn,Telco_Customers$OnlineBackup)
table9<-table(Telco_Customers$Churn,Telco_Customers$OnlineBackup)
barplot(table9,beside = TRUE, main = "Churn - Online Backup", ylim = c(0,2500),
        legend.text = row.names(table9),
        col=c("grey","lightblue"),args.legend = list(x="topright"))

![image](https://user-images.githubusercontent.com/114650133/199351879-50fec7d5-2e48-4abe-8c9e-3dabf30074a4.png)

table(Telco_Customers$Churn,Telco_Customers$DeviceProtection)
table10<-table(Telco_Customers$Churn,Telco_Customers$DeviceProtection)
barplot(table10,beside = TRUE, main = "Churn - Device Protection", ylim = c(0,2500),
        legend.text = row.names(table10),
        col=c("grey","lightblue"),args.legend = list(x="topright"))

![image](https://user-images.githubusercontent.com/114650133/199352079-1a262ce9-ed0f-44e9-a85d-43cdea20ef00.png)

table(Telco_Customers$churn,Telco_Customers$techsupport)
table11<-table(Telco_Customers$Churn,Telco_Customers$TechSupport)
barplot(table11,beside = TRUE, main = "Churn - Tech Support", ylim = c(0,2500),
        legend.text = row.names(table11),
        col=c("grey","lightblue"),args.legend = list(x="topright"))

![image](https://user-images.githubusercontent.com/114650133/199352206-adc59ab8-8d16-42eb-91fe-fb84b18b627e.png)

table(Telco_Customers$churn,Telco_Customers$streamingtv)
table12<-table(Telco_Customers$Churn,Telco_Customers$StreamingTV)
barplot(table12,beside = TRUE, main = "Churn - Streaming TV", ylim = c(0,2500),
        legend.text = row.names(table12),
        col=c("grey","lightblue"),args.legend = list(x="topright"))

![image](https://user-images.githubusercontent.com/114650133/199352307-575d4dac-8c96-4025-b287-35c07ebf6327.png)

table(Telco_Customers$churn,Telco_Customers$streamingmovies)
table13<-table(Telco_Customers$Churn,Telco_Customers$StreamingMovies)
barplot(table13,beside = TRUE, main = "Churn - Streaming Movies", ylim = c(0,2500),
        legend.text = row.names(table13),
        col=c("grey","lightblue"),args.legend = list(x="topright"))

![image](https://user-images.githubusercontent.com/114650133/199352524-d830a472-d868-45ce-853d-2296e9976765.png)

table(Telco_Customers$churn,Telco_Customers$contract)
table14<-table(Telco_Customers$Churn,Telco_Customers$Contract)
barplot(table14,beside = TRUE, main = "Churn - Contract", ylim = c(0,2500),
        legend.text = row.names(table14),
        col=c("grey","lightblue"),args.legend = list(x="topright"))
        
![image](https://user-images.githubusercontent.com/114650133/199352600-e317a969-b510-49c0-8cc4-35663ce559d3.png)

table(Telco_Customers$churn,Telco_Customers$paperlessbilling)
table15<-table(Telco_Customers$Churn,Telco_Customers$PaperlessBilling)
barplot(table15,beside = TRUE, main = "Churn - Paperless Billing", ylim = c(0,3000),
        legend.text = row.names(table15),
        col=c("grey","lightblue"),args.legend = list(x="topright"))

![image](https://user-images.githubusercontent.com/114650133/199352675-d78be3ff-8cf8-4983-8b78-ae2957481f48.png)

table(Telco_Customers$churn,Telco_Customers$paymentmethod)
table16<-table(Telco_Customers$Churn,Telco_Customers$PaymentMethod)
barplot(table16,beside = TRUE, main = "Churn - Payment Method", ylim = c(0,2000),
        legend.text = row.names(table16),
        col=c("grey","lightblue"),args.legend = list(x="topright"))
        
![image](https://user-images.githubusercontent.com/114650133/199352751-ba646fe0-4518-408d-bc2f-b7e31087fded.png)

#### Missing payment method due to crowding. Making adjustments to the factors via levels.


levels(Telco_Customers$PaymentMethod)<-c("Bank transfer","Credit card","Electronic check","Mailed check")


#### Much better.

![image](https://user-images.githubusercontent.com/114650133/199353176-05bf54d8-1da0-42d7-979c-78ad70d29a99.png)

#### Splitting variables into ranges. 

hist(tenure,beside = TRUE, main = "Tenure in months", ylim = c(0,1500), xlim = c(0,90),xlab = "Months")

![image](https://user-images.githubusercontent.com/114650133/199354496-92015bd0-4118-4660-8293-5e25ddcd48fe.png)

Telco_Customers$tenure_age1<-cut(Telco_Customers$tenure, c(0,12,24,48,60,72))
Telco_Customers$tenure_age2<-cut(Telco_Customers$tenure, seq(0,72,12))
Telco_Customers$tenure_age3<-cut(Telco_Customers$tenure, seq(0,72,12), right=FALSE)
Telco_Customers$tenure_age4<-cut(Telco_Customers$tenure, seq(0,72,12), right=FALSE, labels=c(1:6))
levels(Telco_Customers$tenure_age4)<- c("0-12","13-24","25-36","37-48","49-60","61-72")

table17<-table(Telco_Customers$Churn,Telco_Customers$tenure_age4)
barplot(table17,beside = TRUE, xlab='Months',main = "Churn - Tenure ", ylim = c(0,2000),
        legend.text = row.names(table17),
        col=c("grey","lightblue"),args.legend = list(x="topright"))

![image](https://user-images.githubusercontent.com/114650133/199354747-22e6f12b-1acc-4848-8e71-ad604600a396.png)

hist(Telco_Customers$MonthlyCharges, main = "Monthly Charges",xlab = "Dollars", ylim = c(0,1100))

![image](https://user-images.githubusercontent.com/114650133/199354991-53de0f73-03d3-492f-9950-c50ed6d64cf7.png)

table19<-table(Telco_Customers$Churn,Telco_Customers$monthlycharges4)
barplot(table19,beside = TRUE,main = "Churn - Monthly Charges ", ylim = c(0,1500),
        legend.text = row.names(table19),
        col=c("grey","lightblue"),args.legend = list(x="topright"))

![image](https://user-images.githubusercontent.com/114650133/199355101-9d9d337f-7ec7-44e1-8dc9-6ac7709853c4.png)











