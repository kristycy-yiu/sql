DSI SQL Assignment 2, Section 1: Written - Kristy Yiu

Explanation for Type 1 vs Type 2 Slowly Changing Dimensions

Type 1 slowly changing dimensions overwrites the data directly without a history or record of what the previous data may be.
It is not possible to see the changes made or know when the changes were made.

Type 2 slowly changing dimensions retains changes by creating a new row for each change. 
The most recent/updated data is denoted by the address_version column. 
I also included a surrogate key (customer_sk) in addition to the composite key from combining the customer_id and address_version.
This makes it easier to uniquely identify rows.

Both types of slowly changing dimensions are identified clearly in my logical model.
