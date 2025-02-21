
# Loyalty Event Adjust Points

Provides metadata when the event `type` is `ADJUST_POINTS`.

## Structure

`Loyalty Event Adjust Points`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `loyalty_program_id` | `String` | Optional | The Square-assigned ID of the [loyalty program](../../doc/models/loyalty-program.md).<br>**Constraints**: *Maximum Length*: `36` |
| `points` | `Integer` | Required | The number of points added or removed. |
| `reason` | `String` | Optional | The reason for the adjustment of points. |

## Example (as JSON)

```json
{
  "points": 236,
  "reason": null
}
```

