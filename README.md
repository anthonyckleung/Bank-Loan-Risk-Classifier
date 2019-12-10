# Bank Loan Classifier

A bank wants to automate their loan approval process.  They have provided a semi-anonymized dataset containing 606 successful and 76 not successful loans along with their information and transactions. These loans are for existing clients. This could be used to pre approve existing customers and market to them accordingly

This analysis looks into a dataset from a Czech bank. The goal here is to produce a model that can predict whether client should receive a loan or not.

Original [link](https://sorry.vse.cz/~berka/challenge/pkdd1999/berka.htm)

From the original source, client info was divided into 8 tables:
  1. `account` - Static characteristics of the account.
  2. `client` - Describes characteristics (e.g. gender) of the client.
  3. `disposition` - Records that shows how the client is associated with the account.
  4. `permanent_order` -  Describes characteristics of the payment.
  5. `transaction` - Describes transactions for each client. It keeps track the type of payment that was made (e.g., insurance, loan payment, statement payment etc.).
  6. `loan` - Describes the loan granted for a given account.
  7. `credit_card` - Describes the credit card issued to an account.
  8. `demographic` - Describes the demographic characteristics of the client.
  
 The target class is stored in the `loan` table under the `status` column.

In the data table `loan.csv`, the data was preprocessed where the transaction data was aggregated by monthly amount.
