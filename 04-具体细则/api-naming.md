## [Must] 为路径段使用带连字符的小写单独单词
```
  /shipment-orders/{shipment-order-id}
```
这适用于具体的路径段而不是路径参数的名称。 例如{shipment_order_id}可以作为路径参数。

## [Must] 使用snake_case（而不是camelCase）表示查询参数
```
  customer_number, order_id, billing_address
```

## [Should]  首选 Hyphenated-Pascal-Case 表示 HTTP 头字段
这是为了保持文档的一致性（大多数其他 HTTP 头字段遵循这个约定）。 避免 camelCase（不带连字符）。 也有例外，例如一些常见的缩写，如“ID”。
```
  Accept-Encoding
  Apply-To-Redirect-Ref
  Disposition-Notification-Options
  Original-Message-ID
```

## [Must] 资源名称使用复数形式

## [Must] 使用 /api 作为公共 API 路径前缀
如果服务还应该支持非公开的内部API--例如针对具体的操作支持功能 - 添加“/ api”作为基本路径，以清楚地分离公共和非公共API资源
