## [Must] 使用OAuth 2.0保护终端
每个 API 端点都需要使用 OAuth 2.0 进行保护。请参阅官方的 OpenAPI 规范，了解如何在您的 API 规范中指定安全性定义。

## [Must] 定义和分配访问权限（Scopes）
每个 API 都需要定义访问权限，这里称为Scope，每个端点至少需要分配一个Scope。 Scope由每个 API 规范的名称和描述来定义。



Application IDResource IDAccess TypeExamplefulfillment-orderreadfulfillment-order.readfulfillment-orderwritefulfillment-order.writesales-ordersales_orderreadsales-order.sales_order.readsales-ordershipment_orderreadsales-order.shipment_order.read





