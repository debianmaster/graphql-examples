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

