## Business Hours Period

Represents a period of time during which a business location is open.

### Structure

`BusinessHoursPeriod`

### Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `DayOfWeek` | [`string`](/doc/models/day-of-week.md) | Optional | Indicates the specific day  of the week. |
| `StartLocalTime` | `string` | Optional | The start time of a business hours period, specified in local time using partial-time<br>RFC3339 format. |
| `EndLocalTime` | `string` | Optional | The end time of a business hours period, specified in local time using partial-time<br>RFC3339 format. |

### Example (as JSON)

```json
{
  "day_of_week": "SAT",
  "start_local_time": "start_local_time6",
  "end_local_time": "end_local_time8"
}
```

