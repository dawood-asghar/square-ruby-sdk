
# Order Fulfillment Updated Update

Information about fulfillment updates.

## Structure

`Order Fulfillment Updated Update`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `fulfillment_uid` | `String` | Optional | A unique ID that identifies the fulfillment only within this order. |
| `old_state` | [`String (Fulfillment State)`](../../doc/models/fulfillment-state.md) | Optional | The current state of this fulfillment. |
| `new_state` | [`String (Fulfillment State)`](../../doc/models/fulfillment-state.md) | Optional | The current state of this fulfillment. |

## Example (as JSON)

```json
{
  "fulfillment_uid": null,
  "old_state": null,
  "new_state": null
}
```

