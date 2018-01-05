## [Must] 为路径段使用带连字符的小写单独单词

```
  /shipment-orders/{shipment-order-id}
```
这适用于具体的路径段而不是路径参数的名称。 例如{shipment_order_id}可以作为路径参数。

## [Must] 使用snake_case（而不是camelCase）表示查询参数

```
  customer_number, order_id, billing_address
```
wwww