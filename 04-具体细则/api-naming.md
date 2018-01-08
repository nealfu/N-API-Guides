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
为对外公开的公共 API 添加“/api”作为基本路径，以清楚地分离公共和非公共API资源。

## [Must] 避免资源路径最后的/
尾部的斜线不能有特定的语义。资源路径必须提供相同的结果，无论是否具有结尾斜杠。

## [Must] 避免操作（Actions），考虑资源（Resources）
REST是关于资源的，所以请考虑参与Web服务交互的领域实体，并围绕这些实体使用标准的HTTP方法作为操作指示器对您的API进行建模。例如，如果应用程序必须显式锁定文章，以便只有一个用户可以编辑它们，请使用PUT或POST创建文章锁，而不是使用锁定操作。

## [Should] 对完整的业务流程建模
一个 API 应该包含完整的业务流程，包含代表流程的所有资源。这使客户能够理解业务流程，促进业务流程的一致设计，允许从描述和实现的角度来协同作用，并消除API之间的隐式不可见依赖关系。

## [Should] 定义有用的资源
作为一个经验法则，资源的定义应该覆盖客户所有用例的90％。一个有用的资源应包含尽可能多的信息，但尽可能少。支持最后10％的一个好方法是允许客户通过支持过滤和嵌入来指定他们对更多/更少信息的需求。

## [Must] 保证 URL 中无动词
API 描述资源，所以操作应该出现的唯一位置就是 HTTP 方法。 在 URL 中，只能使用名词。不要考虑动作（动词），而可以考虑将消息发送到信箱中：例如，不要在网址中使用动词cancel，而是通过发送一个消息到服务端的cancellations信箱来取消订单。

## [Must] 使用特定领域的资源名称

## [Must] 通过路径段识别资源和子资源

## [Should] 只在必要的情况下使用 UUID

## [May] 考虑使用（非）嵌套 URL

## [Should] 限制资源的数量

## [Should] 限制子资源的层级


