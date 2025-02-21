
# Customer Custom Attribute Filter Value

A type-specific filter used in a [custom attribute filter](../../doc/models/customer-custom-attribute-filter.md) to search based on the value
of a customer-related [custom attribute](../../doc/models/custom-attribute.md).

## Structure

`Customer Custom Attribute Filter Value`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `email` | [`Customer Text Filter Hash`](../../doc/models/customer-text-filter.md) | Optional | A filter to select customers based on exact or fuzzy matching of<br>customer attributes against a specified query. Depending on the customer attributes,<br>the filter can be case-sensitive. This filter can be exact or fuzzy, but it cannot be both. |
| `phone` | [`Customer Text Filter Hash`](../../doc/models/customer-text-filter.md) | Optional | A filter to select customers based on exact or fuzzy matching of<br>customer attributes against a specified query. Depending on the customer attributes,<br>the filter can be case-sensitive. This filter can be exact or fuzzy, but it cannot be both. |
| `text` | [`Customer Text Filter Hash`](../../doc/models/customer-text-filter.md) | Optional | A filter to select customers based on exact or fuzzy matching of<br>customer attributes against a specified query. Depending on the customer attributes,<br>the filter can be case-sensitive. This filter can be exact or fuzzy, but it cannot be both. |
| `selection` | [`Filter Value Hash`](../../doc/models/filter-value.md) | Optional | A filter to select resources based on an exact field value. For any given<br>value, the value can only be in one property. Depending on the field, either<br>all properties can be set or only a subset will be available.<br><br>Refer to the documentation of the field. |
| `date` | [`Time Range Hash`](../../doc/models/time-range.md) | Optional | Represents a generic time range. The start and end values are<br>represented in RFC 3339 format. Time ranges are customized to be<br>inclusive or exclusive based on the needs of a particular endpoint.<br>Refer to the relevant endpoint-specific documentation to determine<br>how time ranges are handled. |
| `number` | [`Float Number Range Hash`](../../doc/models/float-number-range.md) | Optional | Specifies a decimal number range. |
| `boolean` | `TrueClass\|FalseClass` | Optional | A filter for a query based on the value of a `Boolean`-type custom attribute. |
| `address` | [`Customer Address Filter Hash`](../../doc/models/customer-address-filter.md) | Optional | The customer address filter. This filter is used in a [CustomerCustomAttributeFilterValue](../../doc/models/customer-custom-attribute-filter-value.md) filter when<br>searching by an `Address`-type custom attribute. |

## Example (as JSON)

```json
{
  "email": null,
  "phone": null,
  "text": null,
  "selection": null,
  "date": null,
  "number": null,
  "boolean": null,
  "address": null
}
```

