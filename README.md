# salesforce-quickbooks-integration
Salesforce integration with Quickboos

Integration With Quickbooks
https://github.com/jawills/Salesforce-QuickBooks-Integration/tree/master
https://www.youtube.com/watch?v=4lHYeHZRe3k&t=3583s

QBCustomerSync_VF.page
Vf page is created to be used in action button on the account record page. The action it will perform is to sync the account info with quickbook. It uses controller extension : QBCustomerSync_Controller

It will first check if the customer is already created in quickbook then fetch data from there and sync with account.
If not created then it will create the customer in quickbook.

QBData__c
This is custom setting. It contains client id, secrets, auth url etc. These are used to get access and refresh token

QBO_Metadata__mdt
This is custom metadata. It contains base url, company id, minor version etc. These are used to fetch or create customer data in quickbooks

QBCallout
This is the main class for callout.

