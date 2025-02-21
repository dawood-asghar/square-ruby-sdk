
# Booking Creator Details

Information about a booking creator.

## Structure

`Booking Creator Details`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `creator_type` | [`String (Booking Creator Details Creator Type)`](../../doc/models/booking-creator-details-creator-type.md) | Optional | Supported types of a booking creator. |
| `team_member_id` | `String` | Optional | The ID of the team member who created the booking, when the booking creator is of the `TEAM_MEMBER` type.<br>Access to this field requires seller-level permissions.<br>**Constraints**: *Maximum Length*: `32` |
| `customer_id` | `String` | Optional | The ID of the customer who created the booking, when the booking creator is of the `CUSTOMER` type.<br>Access to this field requires seller-level permissions.<br>**Constraints**: *Maximum Length*: `192` |

## Example (as JSON)

```json
{
  "creator_type": null
}
```

