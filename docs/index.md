


**Documentation Map**
- [Customer <a name = "customers"></a>](#customer-)
  - [Boxxe](#boxxe)
    - [**setPrefercustomscript_kw_setpreferredbinue**](#setprefercustomscript_kw_setpreferredbinue)
  - [Highlander <a name = "highlander"></a>](#highlander-)
    - [**customscript_kw_autocontactsearechupdate**](#customscript_kw_autocontactsearechupdate)
    - [**customscript_auto_hcs_projecttaskcreate**](#customscript_auto_hcs_projecttaskcreate)
    - [**customscript_kw_autosalesprices**](#customscript_kw_autosalesprices)
    - [**customscript_kw_delivery_charge_ue**](#customscript_kw_delivery_charge_ue)
    - [**customscript_kw_hide_button_client**](#customscript_kw_hide_button_client)
  - [Artesian Spas <a name="artesianspa"></a>](#artesian-spas-)
    - [**customscript_kw_formulas_1**](#customscript_kw_formulas_1)
  - [DIS <a name ="dis"></a>](#dis-)
  - [Artesian Spas](#artesian-spas)
    - [**customscript_kw_create_so_from_po**](#customscript_kw_create_so_from_po)
    - [**customscript_kw_salesordersummary_ue**](#customscript_kw_salesordersummary_ue)
    - [**customscript_client_kw_warranty_reg**](#customscript_client_kw_warranty_reg)
    - [**customscript_client_kw_warrantyclaim**](#customscript_client_kw_warrantyclaim)
    - [**customscript_client_so_colourrestriction**](#customscript_client_so_colourrestriction)
    - [**customscript_kw_invoice_calculator**](#customscript_kw_invoice_calculator)
    - [**customscript_kw_po_sapshellcol**](#customscript_kw_po_sapshellcol)
    - [**customscript_ue_kw_autowarrantycreation**](#customscript_ue_kw_autowarrantycreation)
    - [**customscript_us_kw_invoice_calculator**](#customscript_us_kw_invoice_calculator)
- [Deployment <a name="deployment"></a>](#deployment-)
- [Git <a name = "git"></a>](#git-)
- [Microsoft Team <a name ="microsoftteam"></a>](#microsoft-team-)
- [:star: Support or Contact](#star-support-or-contact)

# Customer <a name = "customers"></a>


## Boxxe

### **setPrefercustomscript_kw_setpreferredbinue**

Type | name | Id | script 
--- | --- | --- | ---
User Event | `setPreferredBinUE` | customscript_kw_setpreferredbinue |   setPreferredBinUE.js

[find it from our private repo](https://github.com/HighlanderComputingSolution/monthlyBilling/blob/master/docs/setPreferredBinUE.md)




## Highlander <a name = "highlander"></a>

### **customscript_kw_autocontactsearechupdate**

Type | name | Id | script 
--- | --- | --- | ---
Scheduled | `Auto Contract Search Update` | customscript_kw_autocontactsearechupdate |  Schedule_highlander_autoContactSearchUpdate.js


### **customscript_auto_hcs_projecttaskcreate**

Type | name | Id | script 
--- | --- | --- | ---
Scheduled | `Auto Project Task Create` | customscript_auto_hcs_projecttaskcreate |  Schedule_hcs_autoProjectTaskCreate.js




### **customscript_kw_autosalesprices**

Type | name | Id | script 
--- | --- | --- | ---
User Event | `Highlander AutoSalesPrices` | customscript_kw_autosalesprices | UserEventScript_Highlander_autoSalesPrice.js

[find it from our private repo](https://github.com/HighlanderComputingSolution/monthlyBilling/blob/master/docs/UserEventScript_Highlander_autoSalesPrice.md)

### **customscript_kw_delivery_charge_ue**

Type | name | Id | script 
--- | --- | --- | ---
User Event | `Delivery Charge` | customscript_kw_delivery_charge_ue |   deliveryCharge.js

**how to deployment**
1. max __30__ parameters 
2. three different parameters id should start with **custscript_kw_delivery_item_**, **custscript_kw_form_** and **custscriptdelivery_charge_customer_**.  such as : custscript_kw_delivery_item_1 , custscript_kw_form_1, custscriptdelivery_charge_customer_1 . Then, please follow the sequences, such as custscript_kw_hide_button_2
3. choose the delivery item you wanna add into the record based on form id and customer id. please seperate the id by **space**


### **customscript_kw_hide_button_client** 

Type | name | Id | script 
--- | --- | --- | ---
Workflow Action | hide Button Sublist | customscript_kw_hide_button |   hideButtonSublist.js

**how to deployment**
1. max 10 parameters
2. parameters id should start with **custscript_kw_hide_button_**,such as : custscript_kw_hide_button_1. Then, please follow the sequences, such as custscript_kw_hide_button_2
3. find a button id and fill in. for example, press ``ctrl + shfit + c`` in chrome browser, then find button id using cursor.



## Artesian Spas <a name="artesianspa"></a>

### **customscript_kw_formulas_1**

Type | name | Id | script 
--- | --- | --- | ---
Client | `Novuna Finance Client` | customscript_kw_formulas_1 |  Client_kw_novuna_finance.js

**how to deployment**

1. add max 10 parameters
2. parameters id should start with custscript_hld_formula_,such as : custscript_hld_formula_ 1. Then, please follow the sequences, such as custscript_hld_formula_ 2
3. fill in formulas such as: custrecord_hl_hitfin_subsidyamount  = custrecord_hl_subsidy * custrecord_hl_nf_amount


## DIS <a name ="dis"></a>

## Artesian Spas

### **customscript_kw_create_so_from_po**

Type | name | Id | script 
--- | --- | --- | ---
Workflow Action | `Workflow Create SO From PO` | customscript_kw_create_so_from_po |  Workflow_kw_Create_SO_FromPO.js


### **customscript_kw_salesordersummary_ue**

Type | name | Id | script 
--- | --- | --- | ---
User Event | `Sales Order Summary User Event` | customscript_kw_salesordersummary_ue |  UserEvent_kw_SalesOrderSummary.js

### **customscript_client_kw_warranty_reg**

Type | name | Id | script 
--- | --- | --- | ---
Client | `Client Warranty Registration` | customscript_client_kw_warranty_reg |  Client_kw_warrantyRegistration.js


### **customscript_client_kw_warrantyclaim**

Type | name | Id | script 
--- | --- | --- | ---
Client | `Invoice Calculator` | customscript_kw_invoice_calculator |  Client_kw_invoiceCalculate.js




### **customscript_client_so_colourrestriction**

Type | name | Id | script 
--- | --- | --- | ---
Client | `HCS colourRestriction` | customscript_client_so_colourrestriction |  Client_SalesOrder_popup_colourRestrictions.js 


### **customscript_kw_invoice_calculator**

Type | name | Id | script 
--- | --- | --- | ---
Client | `HCS colourRestriction` | customscript_client_so_colourrestriction |  Client_SalesOrder_popup_colourRestrictions.js 


### **customscript_kw_po_sapshellcol**

Type | name | Id | script 
--- | --- | --- | ---
User Event | `Pucharse Order Sap Shell Col` | customscript_kw_po_sapshellcol |  UserEvent_kw_POSapShellCol.js 

### **customscript_ue_kw_autowarrantycreation**

Type | name | Id | script 
--- | --- | --- | ---
User Event | `auto Warranty Creation` | customscript_ue_kw_autowarrantycreation |  UserEvent_kw_autoWarrantyCreation.js


### **customscript_us_kw_invoice_calculator**

Type | name | Id | script 
--- | --- | --- | ---
User Event | `Invoice Calculator` | customscript_us_kw_invoice_calculator |  UserEvent_kw_invoiceCalculate.js






# Deployment <a name="deployment"></a>

there are seperated document for deployment on Microsoft
1. [Email Capture](https://highlander.sharepoint.com/:w:/s/SystemsDevelopment/EbytszPke65Do6XMEPThXzABRtooxNNvVVkhhixQCO4QJA?e=uuWys4): capture email to create record 
- [ ] todo: more flexible for creating different records using same script


2. [IQBlade API](https://highlander.sharepoint.com/:w:/s/SystemsDevelopment/EbytszPke65Do6XMEPThXzABRtooxNNvVVkhhixQCO4QJA?e=uuWys4) : automatically generating customer Record Based on Company House Number

# Git <a name = "git"></a>

this is a [seperated document link](git/git.md) for Git on Github

# Microsoft Team <a name ="microsoftteam"></a>






# :star: Support or Contact  

Having troble with Pages? Check out our [Q&A](q&a/index.md) or [contact support](https://highlanderuk.com/contact/) and we'll help you sort it out.

