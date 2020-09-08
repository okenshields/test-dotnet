## V1 Employee

Represents one of a business's employees.

### Structure

`V1Employee`

### Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Id` | `string` | Optional | The employee's unique ID. |
| `FirstName` | `string` |  | The employee's first name. |
| `LastName` | `string` |  | The employee's last name. |
| `RoleIds` | `IList<string>` | Optional | The ids of the employee's associated roles. Currently, you can specify only one or zero roles per employee. |
| `AuthorizedLocationIds` | `IList<string>` | Optional | The IDs of the locations the employee is allowed to clock in at. |
| `Email` | `string` | Optional | The employee's email address. |
| `Status` | [`string`](/doc/models/v1-employee-status.md) | Optional | - |
| `ExternalId` | `string` | Optional | An ID the merchant can set to associate the employee with an entity in another system. |
| `CreatedAt` | `string` | Optional | The time when the employee entity was created, in ISO 8601 format. |
| `UpdatedAt` | `string` | Optional | The time when the employee entity was most recently updated, in ISO 8601 format. |

### Example (as JSON)

```json
{
  "id": "id0",
  "first_name": "first_name0",
  "last_name": "last_name8",
  "role_ids": [
    "role_ids6",
    "role_ids7",
    "role_ids8"
  ],
  "authorized_location_ids": [
    "authorized_location_ids1"
  ],
  "email": "email6",
  "status": "ACTIVE"
}
```

