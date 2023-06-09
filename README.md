# Data Classification All Objects Report
Ever wondered what the data classification section in the fields settings is about?
<img align="right" src="./img/field_classification.png" width=50% height=50%> It's great news for restricted industries like Healthcare & Life Sciences or Finance. 

Data Classification Metadata lets you flag sensitive fields with the corresponding compliance category, data owner, field usage and sensitivity.
Best of all is that you can report on these classifications and even add your own values if needed.
If you don't want to spend ~15-20 mins to build such a report in your org (as described <a href="https://help.salesforce.com/s/articleView?id=sf.data_classification_metadata_fields.htm&type=5" target="_blank">here</a>
), you can simply deploy my example report to your org with a click of a button. All it contains is a custom report type and an example report for Data Classification which can be filtered by object and classification type.

## Official Documentation
<a href="https://help.salesforce.com/s/articleView?id=sf.data_classification_metadata_fields.htm&type=5" target="_blank">Documentation</a>

### What this Report looks like
![Data Classification Report](./img/report_final.png "Data Classification Report")

### Setting up your own values
![Custom Values](./img/custom_values.png "Custom Values")

## Pre-Requisites / Dependencies
Translation Workbench needs to be enabled in your org to install this report.

## Deploy this to your org

<a href="https://githubsfdeploy.herokuapp.com?owner=UnofficialSalesforceHLS&repo=SFDataClassificationReport">
  <img alt="Deploy to Salesforce"
       src="https://raw.githubusercontent.com/afawcett/githubsfdeploy/master/deploy.png">
</a>

## Prefer SFDX?
1. Clone this repository:
    ```
    git clone https://github.com/UnofficialSalesforceHLS/SFDataClassificationReport.git
    cd SFDataClassificationReport
    ```
1. Authorize your Salesforce org via VSCode or Terminal:
    ```
    sfdx force:auth:web:login
    ```
1. Deploy metadata to your org via VSCode or Terminal (replace YOURUSERNAME with valid one):
    ```
    sfdx force:source:deploy --sourcepath ./force-app -u YOURUSERNAME
    ```