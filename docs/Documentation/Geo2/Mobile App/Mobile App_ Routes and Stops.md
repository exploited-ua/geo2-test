
[Mobile App](../Mobile%20App.md)

# Mobile App: Routes and Stops

- [Introduction](#introduction)
- [Route Statuses](#route-statuses)
- [Starting Route](#starting-route)
- [Current Route](#current-route)
- [Route Creation](#route-creation)
- [Adding/Creating Stops](#adding-creating-stops)
  - [Address Scanning](#address-scanning)
  - [Address Voice Search](#address-voice-search)
  - [Stop details](#stop-details)
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

![App 25.png](../../attachments/ed726956-4fcf-49f6-867a-66a8a8ebf0c4.png)

# Route Statuses

There are three route statuses relevant to the mobile app:

|  **Status**                                                                                 |  **Description**                                                                             |
|:--------------------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------|
| Released <br/>![IMG_6675 1.png](../../attachments/cf4ccb80-ab80-46e2-a20c-558b55922cc1.png) | The route has been released to you.                                                          |
| Started <br/>![](../../attachments/3303e95a-5f5c-4517-b34a-e52edc1e1a9c.png)                | You have started to deliver the route, linking your location tracking to the route.          |
| Completed <br/>![](../../attachments/e332276f-4462-4d08-8a1b-80492ced124f.png)              | You have finished delivering the route.  Location tracking is no longer linked to the route. |

# Starting Route

You can click the 3 dots menu on a route card and press the `Start` button to start the route.  Later, the `Start` button is replaced with the `Pause` button to temporarily pause the route (location tracking for this route will be paused).  To continue the route again, press the `Continue` button. 

![App 36.png](../../attachments/b6d3515e-5f9c-4320-9f7e-217e997a0242.png)![App 37.png](../../attachments/a4c2b183-f912-4646-b1fb-a232d3ee3b7d.png)![App 38.png](../../attachments/7e850b61-3db6-4c62-b4a0-63b35ef8a1e9.png)![App 39.png](../../attachments/8d44ee46-dfde-4c70-84af-1724beb7ef9c.png)

You can also click on the route card to view its details.  At the bottom, you will find the `Start route` button.  After starting the route, the `Start route` button is replaced with the `Complete route` button. To temporarily pause a route press the `arrow` icon near the `Complete route` button and select `Pause route`.  To continue the paused route again, you need to press the `Continue route` button.  It's not possible to continue the route that has been completed already. 

![App 40.png](../../attachments/5dfc52e1-f13f-4737-9914-ea6aec329b13.png)![App 41.png](../../attachments/b27ebe41-a767-4a40-9910-27e96ca4120f.png)![App 42.png](../../attachments/0f29d630-dde5-428b-a74d-520d1c264756.png)![App 43.png](../../attachments/7a9b6958-55ad-47b9-9645-9ba78c0e3973.png)

# Current Route

When you have started a route and location tracking is enabled (the route is not paused), it will be displayed with a green frame around the route card on Routes page.

![App 37.png](../../attachments/a4c2b183-f912-4646-b1fb-a232d3ee3b7d.png)

# Route Creation

Depending on your permissions in the environment, you can create a route in the mobile app as well as in Geo2 Hub. To create a route, you need to press the `Plan route` in Menu or on Routes page. If you do not have any assigned to you routes for today, you will also see the `Plan route` button at the bottom of Map page.

![App 44.png](../../attachments/20086dde-12d4-4923-b9be-942ed604ec12.png)![App 45.png](../../attachments/6e6e9889-8095-4d48-96a5-836dcf164fe9.png)![App 46.png](../../attachments/a05c5f32-8d79-44ec-a942-bc35090fa2e4.png)![App 47.png](../../attachments/8167b20a-5abd-4004-bc1f-e05686c853b6.png)![App 48.png](../../attachments/a43e1495-0c79-4bb9-9566-34106d56bc48.png)

After pressing the button, Plan route page will be displayed where you need to fill in the next fields:

![App 49.png](../../attachments/d5edd074-2ab2-4332-b606-30f9a089a2a6.png)

|  **Fields**    |  **Description**                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |  **Required field**    |
|:---------------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:-----------------------|
| Route key      | Unique route key within an environment.  It will be automatically generated from a date, depot, and trip number if you leave it empty.   It can be a route number, for example, 1, 2, 3, etc.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               | Yes                    |
| Route start    | Before planning your route, you will be asked to use your current geolocation as a route start point but it can be changed. By pressing the Route start field, you can also select other depots from your environment, first stop location (first order recipient’s address), or search address. If you select to search for an address, the Search address dialog will be displayed where you can start typing and selecting an address from the drop-down which appears.  If no suitable match is found, press the `Can't find the address you need?` button and continue entering the address in the relevant address fields manually. Once it is done, press the `Confirm` button. Your address will be saved as a route start.                                                                                                                                                                                         | Yes                    |
| Planned start  | Expected dispatch date/time of the route from the route start location.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     | Yes                    |
| Route end      | By default, the Return to start option is selected for a route end but it can be changed. By pressing the Route end field, you can also select depots from your environment, last stop location (last order recipient’s address), or search address. If you select to search for an address, the Search address dialog will be displayed where you can start typing and selecting an address from the drop-down which appears.  If no suitable match is found, press the `Can't find the address you need?` button and continue entering the address in the relevant address fields manually. Once it is done, press the `Confirm` button. Your address will be saved as a route end and you will be redirected back to Plan route page.                                                                                                                                                                                    | Yes                    |
| Vehicle        | Vehicle assigned to the route. If there are no vehicles yet in your environment, press on the `Tap to add a vehicle` to add it. Vehicle dimensions (“Gross weight”, “Height”, “Width”, and “Length” fields) can be used for route calibration/optimization with vehicle restrictions. The system will factor these dimensions into route building to generate the most efficient outcomes, for example, to avoid bridges with height restrictions, narrow roads unsuitable for wider vehicles, or areas with weight limits that could affect the selected route.                                                                                                                                                                                                                                                                                                                                                            | No                     |
| Driver         | User responsible for the route.  By default, it's a user creating a route from the mobile app.  It can be changed.  Once a route is released, the assigned user sees the route in the mobile app. A driver has permission to start/complete the route. Once the route is started and location tracking enabled, the driver’s location will be displayed [Hub: Routes](../Web-Based%20Hub/Hub_%20Routes.md) and on the [Hub: Analytics](../Web-Based%20Hub/Hub_%20Analytics.md) on Dashboard page, as well as on the recorded [Hub: Vehicle Checks](../Web-Based%20Hub/Hub_%20Vehicle%20Checks.md). The driver’s location can also be optionally displayed on [Hub: Environment Settings](../Web-Based%20Hub/Hub_%20Environment%20Settings.md). However, for POD's, the geolocation of the user who records it will be captured (either the driver or participant). This field is displayed only for Enterprise level users. | No                     |
| Participants   | Up to 2 additional users assigned to the route. Once released, the assigned participant sees the route in the mobile app. While the driver retains the ability to start and complete a route, participants will have access to a route to check the list of stops and create POD's for them. Participants field is displayed only to users with Enterprise subscription level.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              | No                     |

![App 50.png](../../attachments/7d94d7c6-5f03-4214-a6cd-90d4c4c00e35.png)![App 51.png](../../attachments/37bda247-7a9d-47db-b7d8-f7d8135b4826.png)![App 52.png](../../attachments/7bcd4ff4-4552-456f-ba14-94dfa52fed4a.png)![App 53.png](../../attachments/4f636f81-94dc-44d2-ba76-6721bb7b8ba4.png)![App 54.png](../../attachments/366bf743-7348-4046-ab36-cf1bf5c6067e.png)![App 55.png](../../attachments/e5a319bd-791c-4172-a474-f287ce1a8f1a.png)![App 56.png](../../attachments/b5b509e7-eb53-434b-8fad-b2f53e2c60a2.png)

After filling in all the fields, you need to press the `Create` button to save the route data.  You will be redirected to Route view page where you can add stops to the route.

![App 57.png](../../attachments/e2f39d73-2d74-4cfb-9ef0-60a5b9f336d9.png)

# Adding/Creating Stops

Depending on your permissions in the environment settings, you can create or add an existing order to a route in the mobile app or Geo2 Hub. Press the `Add first stop` button at the bottom or `Tap to add a stop` in the stop list on the Route view page. The Search dialog appears, allowing you to type a recipient address and select from the results, use your current location, scan an address, use voice search, or add an existing order.

![App 58.png](../../attachments/7b135545-3e30-476f-b848-0a5146d42f71.png)![App 60.png](../../attachments/6cd7b502-0061-4323-8fb1-a4babd500de7.png)![App 59 (1).png](../../attachments/aab21fd6-306b-4f9c-8089-5a296983aa7b.png)![App 61.png](../../attachments/50282e80-b296-4434-bf17-96293802b43e.png)

Once the address is selected and stop is added, you can continue typing to add more stops.

## Address Scanning

To scan an address, press the `scan` icon on the Tap to add a stop (more stops) search bar or the `Scan address` button on the Search address dialog. The Scan address page will appear. Point your camera steadily at the address and resize the green frame if needed. After scanning, click the `Confirm` button or `Try again` to rescan. Pressing `Confirm` sends the scanned address to find matching results. Select an address from the results to add a stop to the route.

![App 61.png](../../attachments/50282e80-b296-4434-bf17-96293802b43e.png)![App 63.png](../../attachments/2c40ada9-f52a-43ee-881b-e44d854544cc.png)![App 64.png](../../attachments/00f25dc1-39c2-439b-961b-ea9f4815953c.png)![App 65.png](../../attachments/1c985060-c4a4-4178-a539-a6a4dd389e7b.png)

## Address Voice Search

To use voice search for an address, press the `mic` icon on the Tap to add a stop (more stops) search bar or the `Voice search` button in the Search address dialog. The Voice search dialog appears. English is selected by default, but you can change it to any preferred language. Speak the address; the system will recognize it. If the detected address is correct, press `Confirm` to find matching results. Select an address from the results to add a stop to the route. If the detected address is incorrect, press `Try again`.

![App 65.png](../../attachments/1c985060-c4a4-4178-a539-a6a4dd389e7b.png)![App 67.png](../../attachments/3102e6af-b86d-43fc-ac0f-88774c14cba6.png)![App 68.png](../../attachments/6964744e-e1dc-498b-9217-456f4d6d3670.png)![App 66.png](../../attachments/224e3eeb-8342-4f04-96a9-f406595758b3.png)![App 69.png](../../attachments/17a1105d-5c4c-45a8-8867-704e3b39a4d1.png)![App 70.png](../../attachments/5e34cf95-7c6a-4221-bbc7-5a12bf87e04b.png)

## Stop details

Once the stop is added to the route, you can adjust its details:

![App 72.png](../../attachments/744a54f1-7e8a-4c8e-9c05-78db788bad1b.png)![App 73.png](../../attachments/4163040e-97b7-4c86-863e-d315fd9a72cd.png)![App 74.png](../../attachments/78df80b7-47da-4613-a645-ca3d32907e19.png)

|  **Fields**             |  **Description**                                                                                                                                                                                                                                                                              |  **Required fields**    |
|:------------------------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:------------------------|
| Type                    | Delivery or Collection.                                                                                                                                                                                                                                                                       | Yes                     |
| Order key               | Order identifier unique within the environment, for example, an order number 1, 2, 3, 4, etc.  By default, it will be autogenerated from the current date and time. You can click on the `Scan icon` to scan the key.                                                                         | Yes                     |
| Planned                 | For information - date/time when the order is planned to be delivered/collected.  By default, it's current date/time.                                                                                                                                                                         | No                      |
| Committed               | For information - date/time that has been agreed with the customer for delivery/collection. This field is available only for users with Enterprise subscription level.                                                                                                                        | No                      |
| Required from           | For information - from when the customer requires the order to be delivered/collected. It can be used for route optimization with time windows.                                                                                                                                               | No                      |
| Required to             | For information - till when the customer requires the order to be delivered/collected. It can be used for route optimization with time windows.                                                                                                                                               | No                      |
| Stop duration           | The amount of time the delivery vehicle is expected to remain at a route stop. This is used when orders are first brought into a route and, together with drive times, stop durations are intended to lead to route durations that are more realistic than if only drive time was considered. | Yes                     |
| Tab - Recipient details | Optional recipient contact details like contact name, email, phone and mobile phone numbers.                                                                                                                                                                                                  | Yes                     |
| Tab - Packages          | Optional package barcodes.  Barcodes can be either typed in manually or scanned.                                                                                                                                                                                                              | No                      |
| Delivery instructions   | Optional notes for drivers that are shown in the mobile app.  For example, "leave with reception".                                                                                                                                                                                            | No                      |

You can set parcel placement (e.g., "front right" or "left shelf") and optionally add photos for a delivery order by pressing the `Set placement in the vehicle` button at the bottom of the page. Press `Confirm` to save the placement, which can be updated later. The placement and photo count appear on the stop card, and full-size photos can be viewed in Stop details page.

![App 76.png](../../attachments/46c31aaf-53b9-4f66-b8e4-fdcff8058f87.png)![App 75.png](../../attachments/630b1454-56ff-40a2-b932-05ebd26b3f58.png)![App 77.png](../../attachments/e6dddeb7-e2c7-4106-b0ad-d7cd35d81ea1.png)

If a route starts or ends at a depot, it will be used as a stop depot: the route start depot will be populated to the delivery stop, and the route end depot will be populated to the collection stop. If a route does not use a depot as its start or end point but there is a default depot selected in [Hub: Environment Settings](../Web-Based%20Hub/Hub_%20Environment%20Settings.md), it will be used as a stop depot. If there is no default depot, the Depot field inside a stop will be blank.

After adding all stops to the route, you need to press the `Done` button at the top of dialog to run automatic route optimization find the fastest route.  You will be redirected back to Route view page where you can see the added stop cards.  It will be shown on the map when you slide down the bottom sheet.  You can press the `Start route` button to start the route or add more orders.

![App 78.png](../../attachments/aaf20d54-8b18-4e21-9902-5c5bec3dba78.png)![App 79.png](../../attachments/7a1bcffd-0384-4029-a277-f0cd0884e788.png)![App 80.png](../../attachments/d206db24-237c-46ad-9d50-fb9e097d6cc0.png)![App 81.png](../../attachments/c35fd4a0-4270-400f-8d24-ae066b8dae47.png)

## Add Existing Order

To add an existing order to a route, press the `Add existing order` button on Search address dialog. You need to type in the order key or scan it and all the information from this order will be automatically pre-populated to the fields.  You cannot edit the order information on this page. Most of the fields will be disabled for editing. To edit the order, you need to add it to the route, then you can go inside the order and press the `Edit stop` button.

**If a route starts or ends at a depot, orders with depots must match**: the delivery depot must align with the start, and the collection depot with the end. Orders without assigned depots can be added to any route, and if a route does not use a depot as its start or end point, any order, with or without a depot, can be added.

If this order is already assigned to another route, you will be asked to confirm whether you want to move it from one route to another.

![App 83 (1).png](../../attachments/50724fd0-6e9f-4a7a-91af-74b851154204.png)![App 82.png](../../attachments/eda5a3da-9278-497e-8b08-58e5a0ad4aed.png)![App 83.png](../../attachments/c92fffc5-03f5-4301-8951-60fbdf51d655.png)

After adding all stops to the route, you need to press the `Done` button at the top of dialog to run automatic route optimization find the fastest route.  You will be redirected back to Route view page where you can see the added stop cards.  It will be shown on the map when you slide down the bottom sheet.  You can press the `Start route` button to start the route or add more orders.

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
