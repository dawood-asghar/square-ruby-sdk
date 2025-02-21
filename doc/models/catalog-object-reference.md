
# Catalog Object Reference

A reference to a Catalog object at a specific version. In general this is
used as an entry point into a graph of catalog objects, where the objects exist
at a specific version.

## Structure

`Catalog Object Reference`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `object_id` | `String` | Optional | The ID of the referenced object. |
| `catalog_version` | `Integer` | Optional | The version of the object. |

## Example (as JSON)

```json
{
  "object_id": null,
  "catalog_version": null
}
```

