> query

```graphql
{
  account_invoice_line {
    origin_origin_invoice_to_line {
      origin
      state
      vendor_display_name
    }
    product_id
    quantity
    name
    invoice_id
  }
}
```

> relationship
```sh
origin_origin_invoice_to_line -> is 

account_invoice_line . origin → account_invoice . origin
```
> sample output

```json
{
  "data": {
    "account_invoice_line": [
      {
        "origin_origin_invoice_to_line": {
          "origin": "SO003",
          "state": "paid",
          "vendor_display_name": "test@test.com"
        },
        "product_id": 1,
        "quantity": 1,
        "name": "test1",
        "invoice_id": 3
      },
      {
        "origin_origin_invoice_to_line": {
          "origin": "SO001",
          "state": "paid",
          "vendor_display_name": "Administrator"
        },
        "product_id": 1,
        "quantity": 1,
        "name": "test1",
        "invoice_id": 1
      },
      {
        "origin_origin_invoice_to_line": {
          "origin": "SO002",
          "state": "paid",
          "vendor_display_name": "Administrator"
        },
        "product_id": 2,
        "quantity": 3,
        "name": "test2",
        "invoice_id": 2
      },
      {
        "origin_origin_invoice_to_line": {
          "origin": "SO002",
          "state": "paid",
          "vendor_display_name": "Administrator"
        },
        "product_id": 1,
        "quantity": 2,
        "name": "test1",
        "invoice_id": 2
      }
    ]
  }
}
```
