
# Bulk Delete Booking Custom Attributes Request

Represents a [BulkDeleteBookingCustomAttributes](../../doc/api/booking-custom-attributes.md#bulk-delete-booking-custom-attributes) request.

## Structure

`Bulk Delete Booking Custom Attributes Request`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `values` | [`Hash of Booking Custom Attribute Delete Request Hash`](../../doc/models/booking-custom-attribute-delete-request.md) | Required | A map containing 1 to 25 individual Delete requests. For each request, provide an<br>arbitrary ID that is unique for this `BulkDeleteBookingCustomAttributes` request and the<br>information needed to delete a custom attribute. |

## Example (as JSON)

```json
{
  "values": {
    "key0": {
      "booking_id": "booking_id4",
      "key": "key0"
    },
    "key1": {
      "booking_id": "booking_id5",
      "key": "key1"
    },
    "key2": {
      "booking_id": "booking_id6",
      "key": "key2"
    }
  }
}
```

