
# Fulfillment Delivery Details

Describes delivery details of an order fulfillment.

## Structure

`Fulfillment Delivery Details`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `recipient` | [`Fulfillment Recipient Hash`](../../doc/models/fulfillment-recipient.md) | Optional | Information about the fulfillment recipient. |
| `schedule_type` | [`String (Fulfillment Delivery Details Order Fulfillment Delivery Details Schedule Type)`](../../doc/models/fulfillment-delivery-details-order-fulfillment-delivery-details-schedule-type.md) | Optional | The schedule type of the delivery fulfillment. |
| `placed_at` | `String` | Optional | The [timestamp](https://developer.squareup.com/docs/build-basics/working-with-dates)<br>indicating when the fulfillment was placed.<br>The timestamp must be in RFC 3339 format (for example, "2016-09-04T23:59:33.123Z").<br><br>Must be in RFC 3339 timestamp format, e.g., "2016-09-04T23:59:33.123Z". |
| `deliver_at` | `String` | Optional | The [timestamp](https://developer.squareup.com/docs/build-basics/working-with-dates)<br>that represents the start of the delivery period.<br>When the fulfillment `schedule_type` is `ASAP`, the field is automatically<br>set to the current time plus the `prep_time_duration`.<br>Otherwise, the application can set this field while the fulfillment `state` is<br>`PROPOSED`, `RESERVED`, or `PREPARED` (any time before the<br>terminal state such as `COMPLETED`, `CANCELED`, and `FAILED`).<br><br>The timestamp must be in RFC 3339 format<br>(for example, "2016-09-04T23:59:33.123Z"). |
| `prep_time_duration` | `String` | Optional | The duration of time it takes to prepare and deliver this fulfillment.<br>The timestamp must be in RFC 3339 format (for example, "P1W3D"). |
| `delivery_window_duration` | `String` | Optional | The time period after the `deliver_at` timestamp in which to deliver the order.<br>Applications can set this field when the fulfillment `state` is<br>`PROPOSED`, `RESERVED`, or `PREPARED` (any time before the terminal state<br>such as `COMPLETED`, `CANCELED`, and `FAILED`).<br><br>The timestamp must be in RFC 3339 format (for example, "P1W3D"). |
| `note` | `String` | Optional | Provides additional instructions about the delivery fulfillment.<br>It is displayed in the Square Point of Sale application and set by the API.<br>**Constraints**: *Maximum Length*: `550` |
| `completed_at` | `String` | Optional | The [timestamp](https://developer.squareup.com/docs/build-basics/working-with-dates)<br>indicates when the seller completed the fulfillment.<br>This field is automatically set when  fulfillment `state` changes to `COMPLETED`.<br>The timestamp must be in RFC 3339 format (for example, "2016-09-04T23:59:33.123Z"). |
| `in_progress_at` | `String` | Optional | The [timestamp](https://developer.squareup.com/docs/build-basics/working-with-dates)<br>indicates when the seller started processing the fulfillment.<br>This field is automatically set when the fulfillment `state` changes to `RESERVED`.<br>The timestamp must be in RFC 3339 format (for example, "2016-09-04T23:59:33.123Z"). |
| `rejected_at` | `String` | Optional | The [timestamp](https://developer.squareup.com/docs/build-basics/working-with-dates)<br>indicating when the fulfillment was rejected. This field is<br>automatically set when the fulfillment `state` changes to `FAILED`.<br>The timestamp must be in RFC 3339 format (for example, "2016-09-04T23:59:33.123Z"). |
| `ready_at` | `String` | Optional | The [timestamp](https://developer.squareup.com/docs/build-basics/working-with-dates)<br>indicating when the seller marked the fulfillment as ready for<br>courier pickup. This field is automatically set when the fulfillment `state` changes<br>to PREPARED.<br>The timestamp must be in RFC 3339 format (for example, "2016-09-04T23:59:33.123Z"). |
| `delivered_at` | `String` | Optional | The [timestamp](https://developer.squareup.com/docs/build-basics/working-with-dates)<br>indicating when the fulfillment was delivered to the recipient.<br>The timestamp must be in RFC 3339 format (for example, "2016-09-04T23:59:33.123Z"). |
| `canceled_at` | `String` | Optional | The [timestamp](https://developer.squareup.com/docs/build-basics/working-with-dates)<br>indicating when the fulfillment was canceled. This field is automatically<br>set when the fulfillment `state` changes to `CANCELED`.<br><br>The timestamp must be in RFC 3339 format (for example, "2016-09-04T23:59:33.123Z"). |
| `cancel_reason` | `String` | Optional | The delivery cancellation reason. Max length: 100 characters.<br>**Constraints**: *Maximum Length*: `100` |
| `courier_pickup_at` | `String` | Optional | The [timestamp](https://developer.squareup.com/docs/build-basics/working-with-dates)<br>indicating when an order can be picked up by the courier for delivery.<br>The timestamp must be in RFC 3339 format (for example, "2016-09-04T23:59:33.123Z"). |
| `courier_pickup_window_duration` | `String` | Optional | The period of time in which the order should be picked up by the courier after the<br>`courier_pickup_at` timestamp.<br>The time must be in RFC 3339 format (for example, "P1W3D"). |
| `is_no_contact_delivery` | `TrueClass\|FalseClass` | Optional | Whether the delivery is preferred to be no contact. |
| `dropoff_notes` | `String` | Optional | A note to provide additional instructions about how to deliver the order.<br>**Constraints**: *Maximum Length*: `550` |
| `courier_provider_name` | `String` | Optional | The name of the courier provider.<br>**Constraints**: *Maximum Length*: `255` |
| `courier_support_phone_number` | `String` | Optional | The support phone number of the courier.<br>**Constraints**: *Maximum Length*: `17` |
| `square_delivery_id` | `String` | Optional | The identifier for the delivery created by Square.<br>**Constraints**: *Maximum Length*: `50` |
| `external_delivery_id` | `String` | Optional | The identifier for the delivery created by the third-party courier service.<br>**Constraints**: *Maximum Length*: `50` |
| `managed_delivery` | `TrueClass\|FalseClass` | Optional | The flag to indicate the delivery is managed by a third party (ie DoorDash), which means<br>we may not receive all recipient information for PII purposes. |

## Example (as JSON)

```json
{
  "recipient": null,
  "schedule_type": null,
  "deliver_at": null,
  "prep_time_duration": null,
  "delivery_window_duration": null,
  "note": null,
  "completed_at": null,
  "cancel_reason": null,
  "courier_pickup_at": null,
  "courier_pickup_window_duration": null,
  "is_no_contact_delivery": null,
  "dropoff_notes": null,
  "courier_provider_name": null,
  "courier_support_phone_number": null,
  "square_delivery_id": null,
  "external_delivery_id": null,
  "managed_delivery": null
}
```

