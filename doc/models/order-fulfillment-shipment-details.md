## Order Fulfillment Shipment Details

Contains details necessary to fulfill a shipment order.

### Structure

`OrderFulfillmentShipmentDetails`

### Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Recipient` | [`Models.OrderFulfillmentRecipient`](/doc/models/order-fulfillment-recipient.md) | Optional | Contains information on the recipient of a fulfillment. |
| `Carrier` | `string` | Optional | The shipping carrier being used to ship this fulfillment<br>e.g. UPS, FedEx, USPS, etc. |
| `ShippingNote` | `string` | Optional | A note with additional information for the shipping carrier. |
| `ShippingType` | `string` | Optional | A description of the type of shipping product purchased from the carrier.<br>e.g. First Class, Priority, Express |
| `TrackingNumber` | `string` | Optional | The reference number provided by the carrier to track the shipment's progress. |
| `TrackingUrl` | `string` | Optional | A link to the tracking webpage on the carrier's website. |
| `PlacedAt` | `string` | Optional | The [timestamp](#workingwithdates) indicating when the shipment was<br>requested. Must be in RFC 3339 timestamp format, e.g., "2016-09-04T23:59:33.123Z". |
| `InProgressAt` | `string` | Optional | The [timestamp](#workingwithdates) indicating when this fulfillment was<br>moved to the `RESERVED` state. Indicates that preparation of this shipment has begun.<br>Must be in RFC 3339 timestamp format, e.g., "2016-09-04T23:59:33.123Z". |
| `PackagedAt` | `string` | Optional | The [timestamp](#workingwithdates) indicating when this fulfillment<br>was moved to the `PREPARED` state. Indicates that the fulfillment is packaged.<br>Must be in RFC 3339 timestamp format, e.g., "2016-09-04T23:59:33.123Z". |
| `ExpectedShippedAt` | `string` | Optional | The [timestamp](#workingwithdates) indicating when the shipment is<br>expected to be delivered to the shipping carrier. Must be in RFC 3339 timestamp<br>format, e.g., "2016-09-04T23:59:33.123Z". |
| `ShippedAt` | `string` | Optional | The [timestamp](#workingwithdates) indicating when this fulfillment<br>was moved to the `COMPLETED`state. Indicates that the fulfillment has been given<br>to the shipping carrier. Must be in RFC 3339 timestamp format, e.g., "2016-09-04T23:59:33.123Z". |
| `CanceledAt` | `string` | Optional | The [timestamp](#workingwithdates) indicating the shipment was canceled.<br>Must be in RFC 3339 timestamp format, e.g., "2016-09-04T23:59:33.123Z". |
| `CancelReason` | `string` | Optional | A description of why the shipment was canceled. |
| `FailedAt` | `string` | Optional | The [timestamp](#workingwithdates) indicating when the shipment<br>failed to be completed. Must be in RFC 3339 timestamp format, e.g.,<br>"2016-09-04T23:59:33.123Z". |
| `FailureReason` | `string` | Optional | A description of why the shipment failed to be completed. |

### Example (as JSON)

```json
{
  "recipient": {
    "customer_id": "customer_id6",
    "display_name": "display_name8",
    "email_address": "email_address4",
    "phone_number": "phone_number4",
    "address": {
      "address_line_1": "address_line_14",
      "address_line_2": "address_line_24",
      "address_line_3": "address_line_30",
      "locality": "locality4",
      "sublocality": "sublocality4"
    }
  },
  "carrier": "carrier2",
  "shipping_note": "shipping_note6",
  "shipping_type": "shipping_type6",
  "tracking_number": "tracking_number8"
}
```

