
[Mobile App](../Mobile%20App.md)

# Mobile App: Routes and Orders

- [Introduction](#introduction)
- [Route Statuses](#route-statuses)
- [Starting Route](#starting-route)
- [Current Route](#current-route)
- [Route Creation](#route-creation)
- [Adding/Creating Orders](#adding-creating-orders)
  - [Create New Order](#create-new-order)
  - [Add Existing Order](#add-existing-order)
- [Adding/Displaying Breaks](#adding-displaying-breaks)
- [Drag-and-Drop Orders](#drag-and-drop-orders)
- [Calibrating Route](#calibrating-route)
- [Optimizing Route with Time Windows](#optimizing-route-with-time-windows)
- [Optimizing Route without Time Windows](#optimizing-route-without-time-windows)
- [Editing and Deleting Route](#editing-and-deleting-route)
- [Editing and Deleting Order](#editing-and-deleting-order)
- [Vehicle Loading with Photos](#vehicle-loading-with-photos)
- [Navigation](#navigation)
- [Switching Between Stops](#switching-between-stops)
- [Order Packages](#order-packages)
- [Order Products](#order-products)
- [Order Packages with Products](#order-packages-with-products)
- [Recording Stop Duration](#recording-stop-duration)

# Introduction

`Routes` page lets you view routes that have been released to you.  By default, routes planned for the current date are shown, but you can select other dates to show routes for those dates.  The green dot below the date means that you have planned routes assigned to you for this date.

![Routes mob 48.png](../../attachments/76dbfdd3-de1e-48b5-8c9d-26793f7b6b14.png)

# Route Statuses

There are three route statuses relevant to the mobile app:

|  **Status**                                                                                 |  **Description**                                                                             |
|:--------------------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------|
| Released <br/>![IMG_6675 1.png](../../attachments/cf4ccb80-ab80-46e2-a20c-558b55922cc1.png) | The route has been released to you.                                                          |
| Started <br/>![](../../attachments/3303e95a-5f5c-4517-b34a-e52edc1e1a9c.png)                | You have started to deliver the route, linking your location tracking to the route.          |
| Completed <br/>![](../../attachments/e332276f-4462-4d08-8a1b-80492ced124f.png)              | You have finished delivering the route.  Location tracking is no longer linked to the route. |

# Starting Route

You can swipe left over the route and press the `Start` button to start the route.  Later, the `Start` button is replaced with the `Pause` button to temporarily pause the route (location tracking for this route will be paused).  To continue the route again, press the `Continue` button. 

![Routes mob 51.png](../../attachments/0b88dbd3-104d-47fb-b899-23d112e04a32.png)![Routes mob 52.png](../../attachments/e40be4a6-bb66-4921-961b-596b833def66.png)![Routes mob 53.png](../../attachments/581fe917-fcd3-48a8-af87-ed9e636f5141.png)![Routes mob 54.png](../../attachments/8df7d6ab-adfe-482d-aaed-6c33fe5c4bf3.png)![Routes mob 55.png](../../attachments/907d0f66-6013-4463-80f3-865a7b7c9a7b.png)

You can also click on the route card to view its details.  At the top right corner, you will find the `Start` button.  After starting the route, the `Start` button is replaced with the `Pause` and `Complete` buttons - to temporarily pause the route or complete it at all.  To continue the paused route again, you need to press the `Continue` button.  It's not possible to continue the route that has been completed already. 

![Routes mob 56.png](../../attachments/bdbd39f6-008d-4f91-9d91-35391b681680.png)![Routes mob 57.png](../../attachments/f599dee6-cc80-4db5-87dd-fa747b1b850a.png)![Routes mob 58.png](../../attachments/9b64221f-5269-4684-9d9d-bb0f8dd7eb58.png)

# Current Route

When you have started a route, it can be accessed from Home page as well.

![Routes mob 59.png](../../attachments/ec9dc894-43e7-4ec7-b84f-484dfb03f288.png)

# Route Creation

Depending on your permissions in the environment, you can create a route in the mobile app as well as in Geo2 Hub. To create a route, you need to press the `+ (Plus)` button on Home page and choose the `Plan route` option or the `Plan route` button on Home or Routes page.

![Routes mob 1.png](../../attachments/b6b56e40-fd79-4c3e-a4c8-e23c3cebfda9.png)![Routes mob 2.png](../../attachments/b25ef3e4-dd1d-4ac9-be2e-21eda699f7bc.png)![Routes mob 3.png](../../attachments/eeca0649-c9e0-4f17-9576-055016d12738.png)

After pressing the button, Plan route page will be displayed where you need to fill in the next fields:

![Routes mob 5.png](../../attachments/cd8fc5b5-460d-4429-b44a-f11ac0590d4f.png)

|  **Fields**    |  **Description**                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |  **Required field**    |
|:---------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:-----------------------|
| Route key      | Unique route key within an environment.  It will be automatically generated from a date, depot (if it exists in your environment) and trip number if you leave it empty.   It can be a route number, for example, 1, 2, 3, etc.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    | Yes                    |
| Route start    | Before planning your route, you will be asked to use your current geolocation as a route start point but it can be changed. By pressing the Route start field, you can also select other depots from your environment, first stop location (first order recipient’s address), or search address. If you select to search for an address, you will be redirected to a separate page where you can start typing and selecting it from the drop-down which appears.  If no suitable match is found, press the `Can't find the address you need?` button and continue entering the address in the relevant address fields manually. Once it is done, press the `Set address` button. Your address will be saved as a route start and you will be redirected back to Plan route page.                                                                                   | Yes                    |
| Planned start  | Expected dispatch date/time of the route from the depot.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           | Yes                    |
| Route end      | By default, the Return to start option is selected for a route end but it can be changed. By pressing the Route end field, you can also select depots from your environment, last stop location (last order recipient’s address), or search address. If you select to search for an address, you will be redirected to a separate page where you can start typing and selecting it from the drop-down which appears.  If no suitable match is found, press the `Can't find the address you need?` button and continue entering the address in the relevant address fields manually. Once it is done, press the `Set address` button. Your address will be saved as a route end and you will be redirected back to Plan route page.                                                                                                                                 | Yes                    |
| Vehicle        | Vehicle assigned to the route. If there are no vehicles yet in your environment, press on the Vehicle field to add it. Vehicle dimensions (“Gross weight”, “Height”, “Width”, and “Length” fields) can be used for route calibration/optimization with vehicle restrictions. The system will factor these dimensions into route building to generate the most efficient outcomes, for example, to avoid bridges with height restrictions, narrow roads unsuitable for wider vehicles, or areas with weight limits that could affect the selected route.                                                                                                                                                                                                                                                                                                            | No                     |
| Driver         | User responsible for the route.  By default, it's a user creating a route from the mobile app.  It can be changed.  Once a route is released, the assigned user sees the route in the mobile app. A driver has permission to start/complete the route. Once the route is started and location tracking enabled, the driver’s location will be displayed [Hub: Routes](../Web-Based%20Hub/Hub_%20Routes.md) and on the [Hub: Analytics](../Web-Based%20Hub/Hub_%20Analytics.md) on Dashboard page, as well as on the recorded [Hub: Vehicle Checks](../Web-Based%20Hub/Hub_%20Vehicle%20Checks.md). The driver’s location can also be optionally displayed on [Hub: Environment Settings](../Web-Based%20Hub/Hub_%20Environment%20Settings.md). However, for POD's, the geolocation of the user who records it will be captured (either the driver or participant). | No                     |
| Participants   | Up to 2 additional users assigned to the route. Once released, the assigned participant sees the route in the mobile app. While the driver retains the ability to start and complete a route, participants will have access to a route to check the list of stops and create POD's for them. Participants field is displayed only to users with Enterprise subscription level.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     | No                     |

![Routes mob 5.png](../../attachments/cd8fc5b5-460d-4429-b44a-f11ac0590d4f.png)![Routes mob 8.png](../../attachments/1600c755-709f-4b66-837b-a45da6b490ee.png)![Routes mob 9.png](../../attachments/6366af26-ff0b-44b0-ac8d-2aacc7f2bdf7.png)![Routes mob 10.png](../../attachments/61dc6b42-115e-4937-a344-8d6c38a808fa.png)![Routes mob 11.png](../../attachments/3120bc56-5ee4-4cf6-ae8d-eaacbc63d980.png)![Routes mob 6.png](../../attachments/c17ad8d3-73fd-4abe-bcf1-45550caaf962.png)![Routes mob 7.png](../../attachments/c2cac877-df4a-4e87-a69c-a160c6e82106.png)

After filling in all the fields, you need to press the `Continue` button to save the route data.  You will be redirected to Route view page.  You can start a route even if it does not have assigned orders yet.

![Routes mob 12.png](../../attachments/7cd6a6ec-8e89-4f33-b007-18196f01735d.png)

# Adding/Creating Orders

Depending on your permissions in the environment settings, you can create or add an existing order to a route in the mobile app as well as in Geo2 Hub.  You need to press the `Actions` button on Route plan page, and select the `Add order` option.  You will be redirected to Add Order page.

![Routes mob 12.png](../../attachments/7cd6a6ec-8e89-4f33-b007-18196f01735d.png)![Routes mob 13.png](../../attachments/37dd9414-f78d-43fe-a960-570987058ca0.png)

## Create New Order

To create an order, you need to fill in the next fields on Add order page:

![Routes mob 14.png](../../attachments/65291098-6472-4c34-8eff-cafe74b97b83.png)![Routes mob 15.png](../../attachments/6896475c-4bed-414c-8b63-a26f2b38f702.png)

|  **Fields**             |  **Description**                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |  **Required fields**    |
|:------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:------------------------|
| Type                    | Delivery or Collection.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    | Yes                     |
| Order key               | Order identifier unique within the environment, for example, an order number 1, 2, 3, 4, etc.  By default, it will be autogenerated from the current date and time. You can click on the `Scan icon` to scan the key.                                                                                                                                                                                                                                                                                                                                                                      | Yes                     |
| Planned                 | For information - date/time when the order is planned to be delivered/collected.  By default, it's current date/time.                                                                                                                                                                                                                                                                                                                                                                                                                                                                      | No                      |
| Committed               | For information - date/time that has been agreed with the customer for delivery/collection. This field is available only for users with Enterprise subscription level.                                                                                                                                                                                                                                                                                                                                                                                                                     | No                      |
| Required from           | For information - from when the customer requires the order to be delivered/collected. It can be used for route optimization with time windows.                                                                                                                                                                                                                                                                                                                                                                                                                                            | No                      |
| Required to             | For information - till when the customer requires the order to be delivered/collected. It can be used for route optimization with time windows.                                                                                                                                                                                                                                                                                                                                                                                                                                            | No                      |
| Tab - Consignee details | Consignee - contact details and address. By pressing the Recipient address field, you can search for an address. You will be redirected to a separate page where you can use your current location or start typing and selecting it from the drop-down which appears.  If no suitable match is found, press the `Can't find the address you need?` button and continue entering the address in the relevant address fields manually. Once it is done, press the `Set address` button. Your address will be saved as a recipient address and you will be redirected back to Add order page. | Yes                     |
| Delivery instructions   | Optional notes for drivers that are shown in the mobile app.  For example, "leave with reception".                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |                         |

You can set parcel placement (e.g., "front right" or "left shelf") and optionally add photos for a delivery order by pressing the `Set placement in the vehicle` button at the bottom of the page. Press Set to save the placement, which can be updated later. The placement and photo count appear on the stop card, and full-size photos can be viewed in Order details page.

![Routes mob 16.png](../../attachments/127e3699-7b8a-4c3d-bd25-e842d47c01ac.png)![Routes mob 17.png](../../attachments/88edbe0e-e3c9-47b4-ad10-11da6194e657.png)

After filling in all the fields, you need to press the `Add` button to create an order.  You will be redirected back to Route view page where you can see the added order (stop) card.  It will be shown on the map when you slide down the bottom sheet.  You can press the `Start` button to start the route or add more orders.

![Routes mob 18.png](../../attachments/685aaf92-d850-41fc-88b4-efa8cdd45b1c.png)![Routes mob 19.png](../../attachments/978e47f4-b8ac-4d37-9321-de65800ddc03.png)

If a route starts or ends at a depot, it will be used as an order depot: the route start depot will be populated to the delivery order, and the route end depot will be populated to the collection order. If a route does not use a depot as its start or end point but there is a default depot selected in [Hub: Environment Settings](../Web-Based%20Hub/Hub_%20Environment%20Settings.md), it will be used as an order depot. If there is no default depot, the Depot field inside an order will be blank.

## Add Existing Order

To add an existing order to a route, you need to provide the order key and all the information from this order will be automatically pre-populated to the fields.  You cannot edit the order information on this page. Most of the fields will be disabled for editing. You can change only planned, committed, and required from/to date/time. To edit the order, you need to add it to the route, then you can go inside the order and press the `Edit` button.

**If a route starts or ends at a depot, orders with depots must match**: the delivery depot must align with the start, and the collection depot with the end. Orders without assigned depots can be added to any route, and if a route does not use a depot as its start or end point, any order, with or without a depot, can be added.

If this order is already assigned to another route, you will be asked to confirm whether you want to move it from one route to another.

![Routes mob 20.png](../../attachments/7dab1379-b293-4021-8f8b-b34a9d7beb81.png)![Routes mob 21.png](../../attachments/dbf4663b-8d37-42fa-b62a-52a22a335500.png)

After filling in all the fields, you need to press the `Add` button to add an order.  You will be redirected back to Route view page where you can see the added order (stop) card.  It will be shown on the map when you slide down the bottom sheet.  You can press the `Actions` button and optimize the route, press the `Start` button to start the route or add more orders to it.

![Routes mob 22.png](../../attachments/77b7f7b1-f7d1-4249-8269-ab49adaa926f.png)

# Adding/Displaying Breaks

The route view shows breaks alongside order stops. With the required permission in the environment, you can add a break to a route in the mobile app as well as in Geo2 Hub.

To add a break, press the `Actions` button and select the `Add break` option.  You will see a prompt to specify a break in minutes.  By pressing the `Add break` button, it will be added to the end of the stop list.  The break can be dragged-and-dropped to any position in the route. Press `Save` to save changes.  The route will be automatically calibrated, taking new breaks into account.

![Routes mob 24.png](../../attachments/a84a46bb-ee62-4e93-ab3c-a088dce5ad98.png)![Routes mob 23.png](../../attachments/d07c9665-4587-4cb6-b964-ee68811018fd.png)![Routes mob 25.png](../../attachments/adc75b2f-ac80-48ba-a981-e4fb8382fb06.png)![Routes mob 27.png](../../attachments/e40c4f0e-c89c-4cfd-bece-651aaf9ba495.png)![Routes mob 28.png](../../attachments/fbe0a309-67f8-4df8-96c9-d9fff337157d.png)![Routes mob 29.png](../../attachments/fe7d8bc5-a35f-4258-8634-a0dee2dcafa0.png)![Routes mob 30.png](../../attachments/797ac390-ac54-46b5-8916-7c1fb077b0ee.png)![Routes mob 31.png](../../attachments/febd814d-46d1-459a-9309-f4aae9e581fb.png)![Routes mob 32.png](../../attachments/5e0f1471-7ffb-4de3-bff7-77f2112d452c.png)![Routes mob 33.png](../../attachments/45fc6611-2a0a-43cb-b5a6-3fda24d70f96.png)

# Drag-and-Drop Orders

Order (stop) cards could be drag-and-dropped to any position of the route.  For it, you need to press on the order card and move it.  Remember to press the `Save` button to save your changes.  Once saved, a route will be automatically calibrated updating timings and distance.

Route start and end cards cannot be moved.

![Routes mob 34.png](../../attachments/727091ca-6409-488f-9778-05754cf56da8.png)![Routes mob 35.png](../../attachments/0933e593-1b50-4521-b039-8cddea694dd3.png)![Routes mob 36.png](../../attachments/8668f5e0-6985-45f6-8322-255a401d3d44.png)![Routes mob 37.png](../../attachments/fdea1d4c-e14d-46f6-a906-fb232255c375.png)

# Calibrating Route

When you press the `Calibrate` button, the planned timings and distance of the route will be calculated without modifying the order list.  Example: We created 4 orders one by one, didn't change their position, and clicked on the `Calibrate` button.  The route didn't change but the planned time changed.  Remember to press the `Save` button to save these changes. 

The Calibrate option is available if a route has at least 1 order. 

Before route calibration:

![Routes mob 38.png](../../attachments/5ee38bf3-4046-4691-a9d3-b420a6c4f448.png)

After route calibration:

![Routes mob 39.png](../../attachments/00a2ad60-fe70-4fe8-bfcd-3d4a243ab68a.png)

We apply automatic calibration in most cases so you don't need to press `Calibrate`:

- removing orders from a route and pressing `Save`
- adding, changing, deleting a break inside a route and pressing on `Save` if there is at least 1 order
- changing (shuffling) stop order inside a route and pressing on `Save`
- changing start and end points in a route if there is at least 1 order
- changing route planned start time if there is at least 1 order
- changing vehicle in a route if there is at least 1 order
- changing time-at-stop inside order or route stops

Exceptions when we don't apply automatic calibration: 

- adding orders in a route
- editing an order (editing consignee address inside orders)
- manually set up a route inside an order (done from Hub)
- deleting an order on Order details page
- making changes in a depot address or vehicle speed factor

# Optimizing Route with Time Windows

To use the Optimize with time windows option, press the `Actions` button and choose the `Optimize with time windows` option. Route optimization is available when a route has at least 2 orders. Among these orders, there has to be at least 1 order with the provided required time slots (either “Required from”, or “Required to”, or both of them).

![Routes mob 40.png](../../attachments/de4b2f3f-dd5f-4e34-8322-e2d205028369.png)

When you press `Optimize with time windows`, the geo-locations of the assigned depot and the orders will be used to suggest an optimum driving route as well as to match the required time windows for each order. The time window specified using the `Required from` and `Required to` fields inside an order is not considered a hard constraint by the system. That is, the system doesn't fail if the stop cannot be visited during the time window; instead, the system tries to find a route that visits the stop during its time window, but if time-window violations are inevitable, the system tries to find a solution that minimizes the time-window violation time for all stops in the problem.

If you have provided vehicle dimensions (“Gross weight”, “Height”, “Width”, and “Length” fields) for the vehicle assigned to the route, it will be used for optimization with vehicle restrictions. The system will factor these dimensions into route building to generate the most efficient outcomes, for example, to avoid bridges with height restrictions, narrow roads unsuitable for wider vehicles, or areas with weight limits that could affect the selected route.

You are not obliged to accept the suggested order but to save changes, remember to press the `Save` button.

Before route optimization:

![Routes mob 43.png](../../attachments/76d351c4-af13-4a95-88ec-d66db947ae6a.png)![Routes mob 44.png](../../attachments/3430f88c-86b0-48ec-a61b-2507b34ed90d.png)

After route optimization with time windows:

![Routes mob 45.png](../../attachments/f29eb78b-09d6-4cf9-b12c-5ded325c365f.png)![Routes mob 46.png](../../attachments/c1141f3c-e8f1-4ae5-bca1-36e1a9e75361.png)![Routes mob 47.png](../../attachments/f97d38f1-770c-45d0-8ff5-a8c6905620f8.png)

# Optimizing Route without Time Windows

To use the Optimize without time windows option, press the `Actions` button and choose the `Optimize without time windows` option.  Route optimization is available when a route has at least 2 orders.

![Routes mob 40.png](../../attachments/de4b2f3f-dd5f-4e34-8322-e2d205028369.png)

When you press `Optimize without time windows`, the geo-locations of the assigned depot and the orders will be used to suggest an optimum driving route.  The order of the orders may be changed and the planned timings and distance of the route updated.  If you have provided vehicle dimensions (“Gross weight”, “Height”, “Width”, and “Length” fields) for the vehicle assigned to the route, it will be used for optimization with vehicle restrictions. The system will factor these dimensions into route building to generate the most efficient outcomes, for example, to avoid bridges with height restrictions, narrow roads unsuitable for wider vehicles, or areas with weight limits that could affect the selected route.

You are not obliged to accept the suggested order but to save changes, remember to press the `Save` button.

Before optimization without time windows:

![Routes mob 41.png](../../attachments/54063a32-84f6-4267-bc75-8206a389410f.png)

After optimization without time windows:

![Routes mob 42.png](../../attachments/b9460418-87b1-4c7d-b813-e95b08f087ef.png)

# Editing and Deleting Route

By swiping left over a route or using a long press, you can also press the `More` button to open the dialog with the following options: Edit, Delete, and Select multiple routes.  You can create, edit, and delete routes only if you have permission to do it - Manager or Admin role in the current environment.

![Routes mob 60.png](../../attachments/a0656168-4fa3-4711-b357-362d801239de.png)![Routes mob 61.png](../../attachments/1041b47e-1480-4918-80b7-d38b82b7ef2a.png)![Routes mob 62.png](../../attachments/64135e69-3510-484b-af81-18fb5619fe1e.png)

You can also click on the `Actions` button on the Route view page and select the `Edit route` or `Delete route` option.

![Routes mob 63.png](../../attachments/064c05d1-e35d-49b3-94fe-499db661e893.png)

After clicking on the `Edit` button, you will be redirected to Edit route page where you can change some route details and save changes.

After clicking on the `Delete` button, the confirmation dialog will be displayed where you need to confirm the deletion of the route.  It's not possible to delete the route that has the Started or Completed status. 

# Editing and Deleting Order

To edit or permanently delete an order, you need to go to the Route view page and click on the order (stop) card.  You will be redirected to Details page.  At the bottom of the page, you will see the `Edit` and `Delete` buttons.  After clicking on the `Edit` button, you will be redirected to Edit order page where you can make some changes and save them.  After clicking on the `Delete` button, the confirmation dialog will be displayed where you need to confirm the deletion of the order. 

![Routes mob 64.png](../../attachments/9ebc60cb-c273-474e-8e31-6b1a3368a595.png)![Routes mob 65.png](../../attachments/76891f06-c3a6-433f-8637-3ce2ff76cce3.png)

For selecting multiple orders, you need to press the `Actions` button and choose the `Select stops` option.  You can remove them from a route (orders will not be permanently deleted) or create one POD for multiple orders.  If your environment settings don't allow multiple POD's per order per route, it is not possible to select the orders that already have POD's because you can not delete them or create a new POD.

![Routes mob 66.png](../../attachments/89abb22d-f88c-4b16-9f6d-0b83786f28fe.png)![Routes mob 67.png](../../attachments/94ac438e-831b-439b-9541-ba7fc10db3da.png)![Routes mob 68.png](../../attachments/2d49aedf-4842-4186-b1a8-735bba43af4d.png)

# Vehicle Loading with Photos

Once a route is optimized and ready-to-go, you can load your vehicle with the assigned delivery orders by selecting `Load vehicle` from the `Actions` button on Route view page. Stops appear in reverse order to help you load items that will be delivered last first, with **collection orders excluded**. For each stop, you can set parcel placement (e.g., "front right" or "left shelf") and optionally add photos. Press `Done` to save the placement, which can be updated later. Note that new photos will replace the old ones. Once your orders are loaded to the vehicle, press `Finish loading` to return to Route view page.

![Routes mob 72.png](../../attachments/d06d1a30-1aa0-4376-9f3a-c7a4a8c59253.png)![Routes mob 73.png](../../attachments/cdc3fab6-e90c-4b47-b30c-a108d0f68c96.png)![Routes mob 74.png](../../attachments/59597604-5abe-4565-af84-101fe36187d4.png)![Routes mob 75.png](../../attachments/4573e280-f6f4-47cf-8c56-93e397076f91.png)![Routes mob 76.png](../../attachments/f1862d98-fafa-49a0-96db-606f067f3a2d.png)

The placement and photo count appear on the stop card, and full-size photos can be viewed in the Order details page.

![Routes mob 77.png](../../attachments/1903f5ba-20d8-4a75-9216-e0592ffca18e.png)![Routes mob 78.png](../../attachments/781a5f20-942a-43e0-a706-ed7a28edec84.png)

You can also set placement and upload photos when adding or editing an order.

![Routes mob 15.png](../../attachments/6896475c-4bed-414c-8b63-a26f2b38f702.png)![Routes mob 16.png](../../attachments/127e3699-7b8a-4c3d-bd25-e842d47c01ac.png)![Routes mob 17.png](../../attachments/88edbe0e-e3c9-47b4-ad10-11da6194e657.png)

# Navigation

The navigation icon in the top right of Details (of a certain order) page panel lets you jump out to a navigation app (Google Maps, Apple Maps, Waze, etc.) to help you navigate in an unfamiliar area.

![Routes mob 69.png](../../attachments/057a9956-1be2-4211-91ec-5d3c9ddadc67.png)![Routes mob 70.png](../../attachments/e9f53010-4bf9-47cb-9db9-cbb90a9f15d8.png)

# Switching Between Stops

You can see navigation arrows on Order details page above the bottom-screen dialog to quickly switch between route stops. These arrows move dynamically with the bottom sheet as it changes height during scrolling. Next to the arrows, the stop numbers of the previous and next stops are displayed, helping you know which stops you can navigate to. The left arrow is hidden on the first stop, and the right arrow is hidden on the last stop, ensuring navigation options are only shown when applicable. If there is only one stop in the route, no arrows are displayed at all.

![Routes mob 69.png](../../attachments/057a9956-1be2-4211-91ec-5d3c9ddadc67.png)

# Order Packages

You can add packages to an order in [Hub: Orders](../Web-Based%20Hub/Hub_%20Orders.md).  Pre-defined packages will be then displayed on the Order details page in the mobile app with a barcode, description, height, width, depth, volume, and weight depending on the data provided in [Web-Based Hub](../Web-Based%20Hub.md).

![Routes mob 79.png](../../attachments/42d83045-fc0b-4956-bb55-a5e7231f217f.png)

# Order Products

You can add products to an order in [Hub: Orders](../Web-Based%20Hub/Hub_%20Orders.md).  Pre-defined products will be then displayed on the Order details page in the mobile app with a product code, description, quantity, and weight depending on the data provided in [Web-Based Hub](../Web-Based%20Hub.md).

![Routes mob 80.png](../../attachments/faa2ff30-4956-4de1-8794-de0d695ac01d.png)

# Order Packages with Products

You can add packages and products to an order and link them in [Hub: Orders](../Web-Based%20Hub/Hub_%20Orders.md).  Pre-defined packages with products will be then displayed on the Order details page in the mobile app. For a package, a barcode, height, width, depth, volume, and weight can be displayed depending on the data provided in Geo2 Hub. For a product, a product code, description, quantity, and weight can be displayed depending on the data provided in Geo2 Hub. To check products added to a package, press the `Products` button on a package. The list of products added to the package will be displayed. Press `Cross` on the dialog to close it.

![Routes mob 81.png](../../attachments/763a3987-5531-4394-985a-7f0e165434ad.png)![Routes mob 82.png](../../attachments/977f3e3b-5a6e-49d8-a928-8e9660803d50.png)

# Recording Stop Duration

`Record stop duration` setting in [Hub: Environment Settings](../Web-Based%20Hub/Hub_%20Environment%20Settings.md)enables the mobile app’s feature to record the actual time spent at a stop by a driver.

![Screenshot 2025-08-12 at 11.54.59.png](../../attachments/803e50ed-a3aa-495f-b76f-95f3becb18f7.png)

Once enabled, the `Record arrival` button will appear on Order details page within a route in the mobile app. Tapping it records the arrival time for that stop. The button will then be replaced by `Record departure` and `Create POD` options. You can either generate a proof of delivery (POD) before recording the departure or simply log the departure time without a POD.

![Routes mob 83.png](../../attachments/21ccff0c-55ec-4503-8f22-6975b9f0ba6e.png)![Routes mob 84.png](../../attachments/d782bd3f-7fe3-452d-b8a2-c9093ebf1e0f.png)

If you press `Record arrival` and then tap the `Back` button to return to Route view page, you will be prompted to confirm whether you want to record the departure time for this stop.

- Selecting `Yes` will record the departure time.
- Selecting `No` will keep the stop duration counting, and you will be redirected to Route view page.

![Routes mob 85.png](../../attachments/e15ba2e3-99e0-4624-92f9-2f2ece9865fe.png)

If you pause or complete a route, the departure time for the stop where you pressed `Record arrival` will be recorded automatically. The same applies if you fully close the app.

If you press `Record arrival` at a stop and return to Route view page while the stop duration is still counting, you can select multiple stops and press `Record arrival` again.

- If one of the selected stops has an ongoing stop duration, you will be asked whether you want to overwrite the arrival time.
- If none of the selected stops have an ongoing stop duration, you will be asked to confirm whether the departure time for the previous stop should be recorded automatically.
- If selected stops have an ongoing stop duration and you try to select more stops, you will be asked to confirm whether the departure time for the previous stops should be recorded automatically.

![Routes mob 86.png](../../attachments/3b0b8b3a-5b74-41f5-8f3c-15d0566502d1.png)![Routes mob 87.png](../../attachments/cb8957dd-646a-4275-b086-2a2661ac58f9.png)![Routes mob 89.png](../../attachments/95da7876-6097-4476-b8f8-782ba641ede0.png)![Routes mob 88.png](../../attachments/45d57cf9-bf1a-49d7-9308-1715badfc773.png)

We allow **overwriting arrival and departure times for stops** when necessary. Once both arrival and departure times are recorded, the actual stop duration is calculated based on the time difference. This duration appears on the stop card on Route plan page in Hub, allowing you to compare the planned and actual stop duration and take action when necessary.

![Screenshot 2025-08-12 at 12.06.52.png](../../attachments/ea11a523-ea3d-45f1-8c88-a1b67060aa84.png)![Screenshot 2025-08-12 at 12.07.00.png](../../attachments/9e179fe9-f03c-4a78-8f07-b4d309d0ffc4.png)
