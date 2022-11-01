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




















