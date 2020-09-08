## List Cash Drawer Shifts Request

### Structure

`ListCashDrawerShiftsRequest`

### Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `LocationId` | `string` |  | The ID of the location to query for a list of cash drawer shifts. |
| `SortOrder` | [`string`](/doc/models/sort-order.md) | Optional | The order (e.g., chronological or alphabetical) in which results from a request are returned. |
| `BeginTime` | `string` | Optional | The inclusive start time of the query on opened_at, in ISO 8601 format. |
| `EndTime` | `string` | Optional | The exclusive end date of the query on opened_at, in ISO 8601 format. |
| `Limit` | `int?` | Optional | Number of cash drawer shift events in a page of results (200 by<br>default, 1000 max). |
| `Cursor` | `string` | Optional | Opaque cursor for fetching the next page of results. |

### Example (as JSON)

```json
{
  "location_id": "location_id4",
  "sort_order": "DESC",
  "begin_time": "begin_time2",
  "end_time": "end_time2",
  "limit": 172,
  "cursor": "cursor6"
}
```

