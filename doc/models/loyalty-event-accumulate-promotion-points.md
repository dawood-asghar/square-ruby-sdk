
# Loyalty Event Accumulate Promotion Points

Provides metadata when the event `type` is `ACCUMULATE_PROMOTION_POINTS`.

## Structure

`Loyalty Event Accumulate Promotion Points`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `loyalty_program_id` | `String` | Optional | The Square-assigned ID of the [loyalty program](../../doc/models/loyalty-program.md).<br>**Constraints**: *Maximum Length*: `36` |
| `loyalty_promotion_id` | `String` | Optional | The Square-assigned ID of the [loyalty promotion](../../doc/models/loyalty-promotion.md).<br>**Constraints**: *Minimum Length*: `1`, *Maximum Length*: `255` |
| `points` | `Integer` | Required | The number of points earned by the event. |
| `order_id` | `String` | Required | The ID of the [order](../../doc/models/order.md) for which the buyer earned the promotion points.<br>Only applications that use the Orders API to process orders can trigger this event.<br>**Constraints**: *Minimum Length*: `1` |

## Example (as JSON)

```json
{}
```

