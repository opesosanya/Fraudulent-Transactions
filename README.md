# Fraudulent-Transactions
CREATE TABLE FRAUDULENT(
step int,
type varchar(20),	
amount float,
nameOrig varchar(50),	
oldbalanceOrg float,	
newbalanceOrig float,	
nameDest varchar(50),	
oldbalanceDest float,	
newbalanceDest float,	
isFraud int,	
isFlaggedFraud int
);

select * from fraudulent;

copy public.fraudulent
from 'C:\Users\olale\OneDrive\Documents\AVI\Fraudulent Transactions.csv'
delimiter ',' csv header
