## V1 List Employees Request

### Structure

`V1ListEmployeesRequest`

### Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Order` | [`string`](/doc/models/sort-order.md) | Optional | The order (e.g., chronological or alphabetical) in which results from a request are returned. |
| `BeginUpdatedAt` | `string` | Optional | If filtering results by their updated_at field, the beginning of the requested reporting period, in ISO 8601 format |
| `EndUpdatedAt` | `string` | Optional | If filtering results by there updated_at field, the end of the requested reporting period, in ISO 8601 format. |
| `BeginCreatedAt` | `string` | Optional | If filtering results by their created_at field, the beginning of the requested reporting period, in ISO 8601 format. |
| `EndCreatedAt` | `string` | Optional | If filtering results by their created_at field, the end of the requested reporting period, in ISO 8601 format. |
| `Status` | [`string`](/doc/models/v1-list-employees-request-status.md) | Optional | - |
| `ExternalId` | `string` | Optional | If provided, the endpoint returns only employee entities with the specified external_id. |
| `Limit` | `int?` | Optional | The maximum integer number of employee entities to return in a single response. Default 100, maximum 200. |
| `BatchToken` | `string` | Optional | A pagination cursor to retrieve the next set of results for your<br>original query to the endpoint. |

### Example (as JSON)

```json
{
  "order": "DESC",
  "begin_updated_at": "begin_updated_at6",
  "end_updated_at": "end_updated_at4",
  "begin_created_at": "begin_created_at6",
  "end_created_at": "end_created_at8"
}
```

