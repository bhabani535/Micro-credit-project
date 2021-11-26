# Micro-credit-project
Problem Statement: 
    
A Microfinance Institution (MFI) is an organization that offers financial services to low income populations. MFS becomes
very useful when targeting especially the unbanked poor families living in remote areas with not much sources of income. 
The Microfinance services (MFS) provided by MFI are Group Loans, Agricultural Loans, Individual Business Loans and so on.

Many microfinance institutions (MFI), experts and donors are supporting the idea of using mobile financial services (MFS)
which they feel are more convenient and efficient, and cost saving, than the traditional high-touch model used since long 
for the purpose of delivering microfinance services. Though, the MFI industry is primarily focusing on low income families 
and are very useful in such areas, the implementation of MFS has been uneven with both significant challenges and successes.

Today, microfinance is widely accepted as a poverty-reduction tool, representing $70 billion in outstanding loans and a global 
outreach of 200 million clients.

We are working with one such client that is in Telecom Industry. They are a fixed wireless telecommunications network provider.
They have launched various products and have developed its business and organization based on the budget operator model,
offering better products at Lower Prices to all value conscious customers through a strategy of disruptive innovation that
focuses on the subscriber. 

They understand the importance of communication and how it affects a person’s life, thus, focusing on providing their services 
and products to low income families and poor customers that can help them in the need of hour.

They are collaborating with an MFI to provide micro-credit on mobile balances to be paid back in 5 days.The Consumer is believed
to be defaulter if he deviates from the path of paying back the loaned amount within the time duration of 5 days. For the loan
amount of 5 (in Indonesian Rupiah), payback amount should be 6 (in Indonesian Rupiah), while, for the loan amount of 10 
(in Indonesian Rupiah), the payback amount should be 12 (in Indonesian Rupiah).

The sample data is provided to us from our client database. It is hereby given to you for this exercise. In order to improve
the selection of customers for the credit, the client wants some predictions that could help them in further investment and 
improvement in selection of customers. 

OBJECTIVE:
Build a model which can be used to predict in terms of a probability for each loan transaction, whether the customer will be 
paying back the loaned amount within 5 days of insurance of loan. In this case, Label ‘1’ indicates that the loan has been 
payed i.e. Non- defaulter, while, Label ‘0’ indicates that the loan has not been payed i.e. defaulter.  
Points to Remember:
•	There are no null values in the dataset. 
•	There may be some customers with no loan history. 
•	The dataset is imbalanced. Label ‘1’ has approximately 87.5% records, while, label ‘0’ has approximately 12.5% records.
•	For some features, there may be values which might not be realistic. You may have to observe them and treat them with a
    suitable explanation.
•	You might come across outliers in some features which you need to handle as per your understanding. Keep in mind that data 
    is expensive and we cannot lose more than 7-8% of the data. 
    
the Data Description File and The Sample Data for the Modeling.

Variable	                Definition--->Comment

label:	               Flag indicating whether the user paid back the credit amount within 5 days of issuing the loan{1:success,                        0:failure}	
msisdn:	               mobile number of user	
aon:	               age on cellular network in days	
daily_decr30:	       Daily amount spent from main account, averaged over last 30 days (in Indonesian Rupiah)	
daily_decr90:	       Daily amount spent from main account, averaged over last 90 days (in Indonesian Rupiah)	
rental30:	           Average main account balance over last 30 days--->Unsure of given definition
rental90:	           Average main account balance over last 90 days--->Unsure of given definition
last_rech_date_ma:	   Number of days till last recharge of main account	
last_rech_date_da:	   Number of days till last recharge of data account	
last_rech_amt_ma:	   Amount of last recharge of main account (in Indonesian Rupiah)	
cnt_ma_rech30:	       Number of times main account got recharged in last 30 days	
fr_ma_rech30:	       Frequency of main account recharged in last 30 days--->Unsure of given definition
sumamnt_ma_rech30:	   Total amount of recharge in main account over last 30 days (in Indonesian Rupiah)	
medianamnt_ma_rech30:  Median of amount of recharges done in main account over last 30 days at user level (in Indonesian Rupiah)	
medianmarechprebal30:  Median of main account balance just before recharge in last 30 days at user level (in Indonesian Rupiah)	
cnt_ma_rech90:	       Number of times main account got recharged in last 90 days	
fr_ma_rech90:	       Frequency of main account recharged in last 90 days--->Unsure of given definition
sumamnt_ma_rech90:	   Total amount of recharge in main account over last 90 days (in Indonasian Rupiah)	
medianamnt_ma_rech90:  Median of amount of recharges done in main account over last 90 days at user level (in Indonasian Rupiah)	
medianmarechprebal90:  Median of main account balance just before recharge in last 90 days at user level (in Indonasian Rupiah)	
cnt_da_rech30:         Number of times data account got recharged in last 30 days	
fr_da_rech30:          Frequency of data account recharged in last 30 days	
cnt_da_rech90:         Number of times data account got recharged in last 90 days	
fr_da_rech90:          Frequency of data account recharged in last 90 days	
cnt_loans30:           Number of loans taken by user in last 30 days	
amnt_loans30:          Total amount of loans taken by user in last 30 days	
maxamnt_loans30:       maximum amount of loan taken by the user in last 30 days---->There are only two options:
                       5 & 10 Rs., for which the user needs to pay back 6 & 12 Rs. respectively
medianamnt_loans30:    Median of amounts of loan taken by the user in last 30 days	
cnt_loans90:           Number of loans taken by user in last 90 days	
amnt_loans90:          Total amount of loans taken by user in last 90 days	
maxamnt_loans90:       maximum amount of loan taken by the user in last 90 days	
medianamnt_loans90:    Median of amounts of loan taken by the user in last 90 days	
payback30:             Average payback time in days over last 30 days	
payback90:             Average payback time in days over last 90 days	
pcircle:               telecom circle	
pdate:                 date	
