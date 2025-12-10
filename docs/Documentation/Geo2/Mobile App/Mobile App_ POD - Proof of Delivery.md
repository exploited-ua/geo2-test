
[Mobile App](../Mobile%20App.md)

# Mobile App: POD - Proof of Delivery

- [Introduction](#introduction)
- [Planned POD](#planned-pod)
  - [Order Packages](#order-packages)
  - [Order Products](#order-products)
  - [Order Packages with Products](#order-packages-with-products)
- [Ad-hoc/Unplanned POD](#ad-hoc-unplanned-pod)
  - [Order Packages](#order-packages)
  - [Order Products](#order-products)
  - [Order Packages with Products](#order-packages-with-products)
- [POD Custom Fields](#pod-custom-fields)
- [Package-level Failures](#package-level-failures)
- [Package Scanning](#package-scanning)
  - [Adding and Confirming Packages](#adding-and-confirming-packages)
- [Product-level Failures](#product-level-failures)
- [Package-level Failures with Products](#package-level-failures-with-products)

# Introduction

The mobile app lets you record a proof-of-delivery in different circumstances:

- Planned - for an existing order in a planned route
- Ad-hoc - without a planned order
- Ad-hoc - for an existing order that is not part of a route

To record a planned POD, open Order details page and click on the `Create POD` button.

![PODs mob 1.png](../../attachments/0474b375-adf1-47df-99ff-938b661558b5.png)

To record an ad-hoc POD, you can press the `+ (Plus)` button on Home or POD's pages and press the `Create POD` button.

![PODs mob 2.png](../../attachments/ec39ccbd-8066-4f03-b799-69a0c92943e8.png)![PODs mob 3.png](../../attachments/d57bf428-520c-432a-bdf6-b6aa2a582202.png)

You will be redirected to POD creation page.

# Planned POD

![PODs mob 4.png](../../attachments/84e192ef-d645-4d1e-96dc-48f8335fc7b3.png)![PODs mob 5.png](../../attachments/da3ecf25-a9bf-4aeb-8414-7d8745dc101c.png)![PODs mob 6.png](../../attachments/d3e6de96-58fd-4115-9242-690f72a357db.png)

In the Details section, you will see the following fields:

|  **Fields**        |  **Description**                                                                              |  **Required**    |
|:-------------------|:----------------------------------------------------------------------------------------------|:-----------------|
| Type               | Delivery or Collection.                                                                       | Yes              |
| Order key          | Order identifier unique within the environment, for example, an order number 1, 2, 3, 4, etc. | Yes              |
| Contact name       | Name of the person who received the order.                                                    | Yes              |
| Phone number       | Phone number of the person who received the order.                                            | No               |
| Mobile number      | Mobile phone number of the person who received the order.                                     | No               |
| Remarks            | Notes from the driver.                                                                        | No               |
| Notification email | Email address for sending the proof-of-delivery email.                                        | No               |
| Address            | The app uses the address indicated in the order.                                              | Yes              |

Details such as type, key, contact name, email and address will be pre-populated from the order for which you are creating the POD.  You can edit remarks and contact name.

You can select the POD status:

- Successful - order has been successfully delivered/collected.
- Partially successful - part of the order has been delivered/collected.
- Failed - delivery/collection has failed.

![PODs mob 7.png](../../attachments/f5d35f9d-e254-4687-a428-4d82c83af113.png)

In the `Signature` section, record the consignee’s signature by pressing the `Add signature` button and saving the recorded signature.  This is required for successful and partially successful POD's and optional for failed POD's.  In the `Photos` section, you can optionally take or select pictures for the proof-of-delivery.

![PODs mob 8.png](../../attachments/bf25d9cd-ee55-4564-8c78-ebe74a70f05e.png)

After filling in the information, press the `Create POD` button to save the POD.  When the POD is created, you will be redirected back to Order details.  In Order details page, you will see in the right corner:

- a green "done" icon for “Successful” POD status
- a yellow “done” icon for “Partially successful” POD status
- a red “cross” icon for “Failed” POD status

A green “refresh” icon means that there are pending signatures/photos inside a POD. Once they will be successfully uploaded, the icon will be changed accordingly to one of the relevant statuses described above.

![PODs mob 10.png](../../attachments/77dab571-869a-471e-8ad1-88575f9b3926.png)![PODs mob 11.png](../../attachments/67ddfd41-a5fc-410f-b531-1a8bc9ec2b9c.png)![PODs mob 12.png](../../attachments/53e68a14-ecd4-4f8f-b754-dcd51497d740.png)![PODs mob 13.png](../../attachments/fdbc8296-6d59-41db-aaf0-bf06833be471.png)

You can click the POD icon to view POD details. If the order has only one POD, its details will open immediately. If there are multiple POD's, a dialog will appear first so you can select the POD you want to view.

![PODs mob 14.png](../../attachments/3e18c148-d2c1-41c4-9cbb-ca6aad985d56.png)![PODs mob 15.png](../../attachments/953b537e-6774-439a-b1ee-c04612656925.png)![PODs mob 16.png](../../attachments/f07ec1b4-2024-4b58-8310-8dc33fed1733.png)

Also, the created POD will be saved in the POD history on the PODs page.

POD statuses (successful, partially successful, failed, no POD) are also displayed alongside the stops in Route plan page. The POD icon on stop cards on Route view page is not clickable. To view POD details, open the order and click the POD icon, or check the PODs page.

![PODs mob 17.png](../../attachments/0bcb581c-16fd-4530-b80c-54fc7048ff3b.png)![PODs mob 18.png](../../attachments/c8e745b5-f3f2-42ff-83ea-541bf0a8ecf5.png)

## Order Packages

When the order has pre-defined packages, they are displayed in the `Packages` section.  On each package card, a barcode, description, height, width, depth, weight, and volume can be displayed depending on the data provided [Hub: Orders](../Web-Based%20Hub/Hub_%20Orders.md) or API for an order.

![POD 58.png](../../attachments/924687e3-cab1-434d-ae04-1803e3a7f12e.png)

When the order doesn't have packages, the `Packages` section is collapsed by default.  You can expand it, provide the number of successfully delivered/collected packages out of the total planned and add packages by typing a barcode manually or scanning package barcodes.  

![POD 59.png](../../attachments/00b40793-9c03-4d79-bdc6-760a6f73a518.png)![POD 60.png](../../attachments/ce72f28d-88ba-4af4-9e07-1fc62d83f6e9.png)

When you create a POD for multiple orders, the `Packages` section is hidden.

![POD 62.png](../../attachments/a0240251-7a26-4fe0-b039-03bd428e67e9.png)![POD 63.png](../../attachments/ddee7691-6bd3-41f8-a313-a7ade9acd555.png)

By default, packages are marked as delivered (checkboxes are selected). See [Page not accessible](../../../../../../../../Page%20not%20accessible/Page%20not%20accessible.md) on marking packages as failed.

![POD 60.png](../../attachments/ce72f28d-88ba-4af4-9e07-1fc62d83f6e9.png)

## Order Products

When the order has pre-defined products, they are displayed in the `Products` section.  On each product card, a product code, description, quantity, and weight can be displayed depending on the data provided in [Hub: Orders](../Web-Based%20Hub/Hub_%20Orders.md) or via the API for an order.

![POD 64.png](../../attachments/37742c86-7685-4b3f-8929-72635db99b71.png)

When the order doesn't have products, the `Products` section is not displayed.  When you create a POD for multiple orders, the `Products` section is hidden. By default, products are marked as delivered (checkboxes are selected). See [Page not accessible](../../../../../../../../Page%20not%20accessible/Page%20not%20accessible.md) on marking products as failed.

## Order Packages with Products

When the order has pre-defined products and packages linked, they are displayed in the `Packages and products` section.  For a package, a barcode, height, width, depth, volume, and weight can be displayed depending on the data provided in Geo2 Hub. For a product, a product code, description, quantity, and weight can be displayed depending on the data provided in Geo2 Hub. To check products added to a package, press the `Products` button on a package. The list of products added to the package will be displayed. Press `Back` to return to Create POD page.

![POD 66.png](../../attachments/23012e02-f8f9-4d82-bd59-d3d68f514009.png)![POD 65.png](../../attachments/58d38067-71d4-4b1d-84ed-2b872935c72b.png)

When you create a POD for multiple orders, the `Packages and products` section is hidden. By default, packages with products inside are marked as delivered (checkboxes are selected). See [Page not accessible](../../../../../../../../Page%20not%20accessible/Page%20not%20accessible.md) on marking packages with products as failed.

# Ad-hoc/Unplanned POD

You can create an ad-hoc POD for an existing order by specifying its key.  If the order key does not yet exist, a skeleton order will be created in the background (depending on [Hub: Environment Settings](../Web-Based%20Hub/Hub_%20Environment%20Settings.md)).  If you provide the key of an existing order, details such as type, key, contact name, email, and address are pre-populated.  You can edit remarks and contact name.

![POD 67.png](../../attachments/90a7573b-9e5b-44fa-ad00-19633912d015.png)![POD 68.png](../../attachments/f61920d7-3512-46cd-831d-d95eb7409b2f.png)

If the order does not exist yet, fill in the following fields in the `Details` section:

|  **Fields**        |  **Description**                                                                                                                                                                                |  **Required**    |
|:-------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:-----------------|
| Type               | Delivery or Collection                                                                                                                                                                          | Yes              |
| Order key          | Order identifier unique within the environment, for example, an order number 1, 2, 3, 4, etc. You can click on the `Scan` icon to scan the key.  It is possible to provide multiple order keys. | Yes              |
| Contact name       | Name of the person who received the order                                                                                                                                                       | Yes              |
| Phone number       | Consignee phone number                                                                                                                                                                          | No               |
| Mobile number      | Consignee mobile phone number                                                                                                                                                                   | No               |
| Remarks            | Notes from the driver                                                                                                                                                                           | No               |
| Notification email | Email address for sending the proof-of-delivery email                                                                                                                                           | No               |
| Address            | The app uses the current device location. This can be edited.                                                                                                                                   | Yes              |

You can select the POD status:

- Successful - order has been successfully delivered/collected.
- Partially successful - part of the order has been delivered/collected.
- Failed - delivery/collection has failed.

![POD 69.png](../../attachments/dbbeaa69-0eb5-48b6-8011-8cd1a3c0e1a3.png)

In the `Signature` section, you need to record a consignee signature by pressing the `Add signature` button and saving the recorded signature.  This is required for successful and partially successful POD's and optional failed POD's.  In the `Photos` section, you can optionally take or select pictures for the proof-of-delivery.

After filling in all the data, press the `Create POD` button to save the POD.  After the POD is created, it will be saved in POD history on POD's page.  Icons on the right side of each POD means:

- a green "done" icon for “Successful” POD status
- a yellow “done” icon for “Partially successful” POD status
- a red “cross” icon for “Failed” POD status

![POD 70.png](../../attachments/b4f96969-4021-4696-9396-94c2f5249125.png)

## Order Packages

When the order has pre-defined packages (ad-hoc POD for existing order), they are displayed in the `Packages` section.  On each package card, a barcode, description, height, width, depth, weight, and volume can be displayed depending on the data provided [Hub: Orders](../Web-Based%20Hub/Hub_%20Orders.md) or API for an order.

![POD 58.png](../../attachments/924687e3-cab1-434d-ae04-1803e3a7f12e.png)

When the order doesn't have packages (ad-hoc POD for either existing order without pre-defined packages or not yet existing order), the `Packages` section is collapsed by default.  You can expand it, provide the number of successfully delivered/collected packages out of the total planned, and add packages by typing a barcode manually or scanning package barcodes.

![POD 59.png](../../attachments/00b40793-9c03-4d79-bdc6-760a6f73a518.png)![POD 60.png](../../attachments/ce72f28d-88ba-4af4-9e07-1fc62d83f6e9.png)

When you create a POD for multiple orders, the `Packages` section is hidden.

![POD 71.png](../../attachments/50bcc85d-e501-4610-80ba-42c8410cf6cf.png)![POD 72 (1).png](../../attachments/e02ff864-441f-42fd-8f38-2299bf1e26bd.png)

By default, packages are marked as delivered (checkboxes are selected). See [Page not accessible](../../../../../../../../Page%20not%20accessible/Page%20not%20accessible.md)on marking packages as failed.

![POD 60.png](../../attachments/ce72f28d-88ba-4af4-9e07-1fc62d83f6e9.png)

## Order Products

When the order has pre-defined products (ad-hoc POD for existing order key), they are displayed in the `Products` section.  On each product card, a product code, description, quantity, and weight can be displayed depending on the data provided [Hub: Orders](../Web-Based%20Hub/Hub_%20Orders.md) or API for an order.

![POD 64.png](../../attachments/37742c86-7685-4b3f-8929-72635db99b71.png)

When the order doesn't have products, the `Products` section is not displayed.  It is not possible to add them via the mobile app. When you create a POD for multiple orders, the `Products` section is hidden. By default, products are marked as delivered (checkboxes are selected). See [Page not accessible](../../../../../../../../Page%20not%20accessible/Page%20not%20accessible.md) on marking products as failed.

## Order Packages with Products

When the order has pre-defined products and packages linked, they are displayed in the `Packages and products` section.  For a package, a barcode, height, width, depth, volume, and weight can be displayed depending on the data provided in Geo2 Hub. For a product, a product code, description, quantity, and weight can be displayed depending on the data provided in Geo2 Hub. To check products added to a package, press the `Products` button on a package. The list of products added to the package will be displayed. Press `Back` to return to Create POD page.

![POD 65.png](../../attachments/58d38067-71d4-4b1d-84ed-2b872935c72b.png)![POD 66.png](../../attachments/23012e02-f8f9-4d82-bd59-d3d68f514009.png)

When you create a POD for multiple orders, the `Packages and products` section is hidden. By default, packages with products inside are marked as delivered (checkboxes are selected). See [Page not accessible](../../../../../../../../Page%20not%20accessible/Page%20not%20accessible.md) on marking packages with products as failed.

# POD Custom Fields

In the Environment settings, you can set up custom fields to collect additional information in POD's.  Here is an example:

- Ask for the driver's name
- Ask if the parcel is intact

![Screenshot 2025-03-18 at 16.57.23.png](../../attachments/4ab51b69-71c1-411a-aa1b-b1a7c780a022.png)

That's how the fields would look when recording a POD:

![POD 73.png](../../attachments/eae060bf-ec61-4b02-91b5-a1f20df5b3c0.png)

# Package-level Failures

If the order has pre-defined packages, they will be displayed on Create POD page, marked as delivered by default (checkboxes are selected).  You can de-select a package to mark that it was not delivered.  You will see a prompt to specify the failure reason code for it.  The POD status will be automatically changed from Successful to Partially successful and the failure reason code from the package level will be populated to the general POD level.  The failure code for the package will be highlighted in red colour.  You can press it to select another code.

You can first select the Partially successful status, a general failure reason code for the POD, and after that, de-select packages.  The general failure reason code will be populated to the package level, but you can change it for each package individually.

![POD 74.png](../../attachments/7b01fd30-078a-43d6-a92d-528662a626f0.png)![POD 75.png](../../attachments/a1e6859b-a56d-403a-9eb1-e7df9741633f.png)![POD 76.png](../../attachments/ef208850-fe02-4264-8aa2-a3841fa9c9b1.png)![POD 77.png](../../attachments/df14edce-b05a-410c-8523-d35dbe7236c7.png)![POD 78.png](../../attachments/04530c75-d99f-49d6-91f1-8ddd748a49ed.png)

If all packages have failed, you can either de-select each manually by unticking the checkboxes or by pressing the `Deselect all` button.  You will see the `Select failure reason code` button on each package to specify the failure reason code.  You can press a package card to provide a failure reason code.  You will see two options - `Apply for all failed packages` or `Apply for selected package`. If `Apply for all failed packages` is selected, the failure reason code will be populated for all packages. If `Apply for selected package` is selected, the failure reason code will be populated only for the selected package. You can press other package cards and select another failure reason for them. You will see the same options - `Apply for all failed packages` (those without a reason code so far) or `Apply for selected package`. The last selected failure reason code will be saved for the general POD level. The POD status will be automatically changed from Successful to Failed and the failure reason code from the package level will be populated to the general POD level.  The failure code for the packages will be highlighted in red colour.  You can press it to select another code (for example, to provide an individual code for each package).

You can first select a Failed status and a general failure reason code for the POD.  All packages will be de-selected automatically.  The general failure reason code will be populated to the package level, but you can change it for each package individually.

![POD 79.png](../../attachments/9d6c30af-6a69-42c4-ac47-04a93ef3f79e.png)![POD 80.png](../../attachments/7acc9aca-3714-4e1c-b550-de55b3bcd9e7.png)![POD 81.png](../../attachments/88fb628d-9d73-4e61-ac0a-3bbe129766ac.png)![POD 82.png](../../attachments/1ccf51ff-f040-4823-8f70-d17af5ea3be5.png)

To mark all unticked (de-selected) packages as successful again, press the `Select all` button - the POD status will be changed to Successful as well.

# Package Scanning

Package scanning serves multiple purposes:

- to add packages to an order when it does not have them yet
- to validate whether a package belongs to the order, when the order has packages pre-defined
- to specify packages that have been delivered, both when they are pre-defined and when they have just been added in the course of POD creation

## Adding and Confirming Packages

If the order has no pre-defined packages, it is possible to scan barcodes to add packages by pressing the `Scan` button.  You will be redirected to Scan barcode page.  Point your camera steadily at the barcode or QR code and it will be scanned.  The scanned code will be displayed under the title `Scanned barcodes`.  You can press:

- `Red minus` icon to remove this barcode
- `Scan more` button to scan more barcodes
- `Done` button to complete scanning

![POD 83.png](../../attachments/c2d6b039-8cdb-4ae0-9f18-ae0dedaba706.png)![POD 84.png](../../attachments/8728b46d-37af-46ed-8274-df38199e1481.png)

Press the `Scan more` button when the device camera is over a new barcode.  If you try to scan the same barcode, you will get an error message.

![POD 85.png](../../attachments/242b0353-7d95-429a-80e6-1960a4ca2ed7.png)![POD 86.png](../../attachments/2ae409c2-f647-457f-a742-d71a4feaf037.png)

Once all required barcodes are scanned, press the `Done` button to be redirected to Create POD page.  All scanned barcodes will be ticked (selected) as successfully delivered/collected.  If some of them have not been delivered, you can untick (de-select them) and provide a failure reason code.

![POD 87.png](../../attachments/10e6d9a5-d37a-4766-bd45-fdc5bc7c315d.png)

On Create POD page, you can also press the red minus icon to remove packages.

If the order has pre-defined packages, it is also possible to scan barcodes to verify packages or confirm them by pressing the `Scan` button.  You will be redirected to Scan barcode page.  Point your camera steadily at the barcode or QR code and it will be scanned.  The scanned code will be displayed under the title `Scanned barcodes`.  You can press:

- `Red minus` icon to remove this barcode
- `Scan more` button to scan more barcodes
- `Done` button to complete scanning

If you try to scan the barcode that does not belong to this order, you will get an error message.

![POD 88.png](../../attachments/684ed1e9-c12e-4751-a9d9-af412ed45d2b.png)![POD 89.png](../../attachments/97490571-5687-4ce2-9a95-4b51d83281c9.png)![POD 90.png](../../attachments/205ccb5b-cacc-4753-9923-52cb7b2c42db.png)

Once all barcodes are scanned, press the `Done` button to be redirected to Create POD page.  All scanned barcodes will be ticked (selected) as successfully delivered/collected.  If some of them have not been delivered, you can untick (de-select them) and provide a failure reason code.

If you do not scan any of pre-defined packages, you will see a prompt asking if you want to continue scanning as there are not confirmed packages. By pressing the `Complete` button, you will be redirected back to POD page. Not confirmed/scanned packages will be marked as failed. You need to select a failure reason code for it.

![POD 91.png](../../attachments/6fa922f1-35cc-4f85-aa97-92f0585b2694.png)![POD 92.png](../../attachments/d8066557-0e05-4927-972e-e68b2708a01b.png)![POD 93.png](../../attachments/69a5c277-0d62-4302-ab2c-5e833817fb17.png)![POD 94.png](../../attachments/536c9aa6-79c7-4a38-b2c5-0d620676979f.png)

# Product-level Failures

If the order has pre-defined products, they are displayed on Create POD page, marked as delivered by default (checkboxes are selected).  You can de-select a product to mark that it was not delivered.  You will see a prompt to specify the failure reason code for it and the failed quantity out of the planned total.  The POD status will be automatically changed from Successful to Partially successful and the failure reason code from the product level will be populated to the general POD level.  The failure code for the product will be highlighted in red colour.  You can press it to select another code or change the failed quantity.

You can first select the Partially successful status, a general failure reason code for the POD, and after that, de-select products.  The general failure reason code will be populated to the product level, but you can change it for each product individually.

![POD 95.png](../../attachments/95eca24e-7a68-44f5-91c0-05004ed942df.png)![POD 96.png](../../attachments/97cec4a7-90e9-4c19-9a50-34546d2c62c0.png)![POD 97.png](../../attachments/ef955109-cec6-4b5d-9f85-28b8778c19a7.png)![POD 98.png](../../attachments/03d0821e-2569-4bd4-a08c-68f14078c811.png)

If all products have failed, you can either de-select each manually by unticking the checkboxes or by pressing the `Deselect all` button.  You will see `Select failure reason code` button on each product to specify the failure reason code.  You can press on it to provide a failure reason code and failed quantities.  You will see two options - `Apply for all failed products` or `Apply for selected product`. If `Apply for all failed products` is selected, the failure reason code will be populated for all products. Full quantities of other products will be automatically failed. If `Apply for selected product` is selected, the failure reason code will be populated only for the selected product. You can press other product cards and select another failure reason for them and a failed quantity. You will see the same options - `Apply for all failed products` (those without a reason code yet) or `Apply for selected product`. The last selected failure reason code will be saved for the general POD level. The POD status will be automatically changed from Successful to Failed and the failure reason code from the product level will be populated to the general POD level.  The failure code for the products will be highlighted in red colour.  You can press it to select another code (for example, to provide an individual code for each product) and the failed quantity.  If not the full quantity of the product fails, the general status will be changed to Partially successful.

You can first select a Failed status and a general failure reason code for the POD.  All products will be de-selected automatically.  The general failure reason code will be populated to the product level, but you can change it for each product individually.

![POD 99.png](../../attachments/15a52057-9043-43ae-b0cc-0188180dd8c4.png)![POD 101.png](../../attachments/4b53d963-5e65-4638-9f57-390bbe884ed2.png)![POD 100.png](../../attachments/0f235bf1-67d2-46ab-8528-9e8f31ea062f.png)![POD 102.png](../../attachments/c64a89c4-ee2a-4707-9740-fcf9e82e5ece.png)

To mark all unticked (de-selected) products as successful again, press the `Select all` button - the POD status will be changed to Successful as well.

# Package-level Failures with Products

If the order has pre-defined packages with products linked, they will be displayed on Create POD page, marked as delivered by default (checkboxes are selected).  You can de-select a package to mark that it was not delivered.  You will see a prompt to specify the failure reason code for it.  The POD status will be automatically changed from Successful to Partially successful and the failure reason code from the package level will be populated to the general POD level.  The failure code for the package will be highlighted in red colour.  You can press it to select another code.  All products added to the package will be marked as failed with the full quantities failed.

You can first select the Partially successful status, a general failure reason code for the POD, and after that, de-select packages.  The general failure reason code will be populated to the package level, but you can change it for each package individually.

![POD 103.png](../../attachments/c6d4d671-93ea-4ee4-9274-bf8528cb1bc4.png)![POD 104.png](../../attachments/1cfa0ecf-e984-4e03-b592-db68d539935e.png)![POD 104 (1).png](../../attachments/6e867a6e-4fa6-4197-bedf-e3a17c5d7478.png)![POD 105.png](../../attachments/7f6c9a5b-559f-45c5-b62e-1aaf0c9f5414.png)

It is possible to press the Products button on a package to mark that only part of the product failed. The product will have a “Partially successful” status and a failure reason code will be highlighted in orange colour. The package status will be also automatically changed to “Partially successful”.

![POD 106.png](../../attachments/fe252ece-5e7e-495b-ba5b-cd338304551f.png)![POD 107.png](../../attachments/d6de6e62-71ac-4609-bd3f-036b3bd7a6d5.png)![POD 108.png](../../attachments/d146dc18-a693-4f5c-b9c1-8993e192e9c3.png)![POD 109.png](../../attachments/1dbf9f6b-af4e-457a-9d9f-020940e90d15.png)

If all packages with products have failed, you can either de-select each manually by unticking the checkboxes or by pressing the `Deselect all` button.  You will see the `Select failure reason code` button on each package and product to specify the failure reason code.  You can press on a package to provide a failure reason code.  You will see two options - `Apply for all failed packages` or `Apply for selected package`. If `Apply for all failed packages` is selected, the failure reason code will be populated for all packages and products linked to them. If `Apply for selected package` is selected, the failure reason code will be populated only for the selected package and products linked to it.

![POD 112.png](../../attachments/19dc3b27-fbae-431b-9762-0169bc7e5c20.png)![POD 111.png](../../attachments/fedb4400-722d-48c8-80a9-2bf223d414cc.png)![POD 110.png](../../attachments/73376e5a-689d-41a1-aa71-ee506b374732.png)![POD 113.png](../../attachments/c2d5b6fd-ddab-4ca7-8bb1-1ae6d4aad441.png)![POD 114.png](../../attachments/67263d7e-4410-4762-b641-f9e81e881ad4.png)

You can press other package cards and select another failure reason for them. You will see the same options - `Apply for all failed packages` (those without a reason code yet) or `Apply for selected package`. The last selected failure reason code will be saved for the general POD level.

![POD 115.png](../../attachments/d92006ef-8234-4623-a260-f6b3d884d1d3.png)![POD 116.png](../../attachments/c63944a2-73f1-404f-b1ad-4d8ffb42d2d9.png)![POD 117.png](../../attachments/877c8d3e-8e99-4ef9-8809-2855df972fca.png)![POD 118.png](../../attachments/924c62cf-7cdf-43c1-9f0d-1b985c0160d4.png)![POD 119.png](../../attachments/f3801075-5acb-4bc7-919f-77be48196923.png)

The failure code for the packages and products inside them will be highlighted in red colour.  You can press it to select another code (for example, to provide an individual code for each product) and the failed quantity.  If not the full quantity of the product fails, the general status will be changed to Partially successful.

You can first select a Failed status and a general failure reason code for the POD.  All packages and products will be de-selected automatically.  The general failure reason code will be populated to the package and product level, but you can change it for each product individually.
