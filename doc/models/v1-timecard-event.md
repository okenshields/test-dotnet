## V1 Timecard Event

V1TimecardEvent

### Structure

`V1TimecardEvent`

### Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Id` | `string` | Optional | The event's unique ID. |
| `EventType` | [`string`](/doc/models/v1-timecard-event-event-type.md) | Optional | Actions that resulted in a change to a timecard. All timecard<br>events created with the Connect API have an event type that begins with<br>`API`. |
| `ClockinTime` | `string` | Optional | The time the employee clocked in, in ISO 8601 format. |
| `ClockoutTime` | `string` | Optional | The time the employee clocked out, in ISO 8601 format. |
| `CreatedAt` | `string` | Optional | The time when the event was created, in ISO 8601 format. |

### Example (as JSON)

```json
{
  "id": "id0",
  "event_type": "API_CREATE",
  "clockin_time": "clockin_time6",
  "clockout_time": "clockout_time4",
  "created_at": "created_at2"
}
```

