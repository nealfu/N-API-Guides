## [Should] 数组名称应该为复数
为了表明它们包含多个值，应该复数化数组名称。 这意味着对象名称应该是单数。

## [Must] 布尔属性值不能为空
JSON属性不得显示为空值。 一个布尔值本质上是一个封闭的枚举值，true和false。 如果内容具有有意义的空值，则强烈倾向于用枚举的命名值或状态来替换布尔值 - 例如用true或false接受的_terms_and_conditions可以用具有值yes，no和unknown的terms_and_conditions替换。

## [Should] 属性为 Null 时，不应该参加序列化
常用的 Swagger / OpenAPI 不支持空字段值（如果未标记为必填，则允许完全忽略该字段）。 但是，这并不妨碍客户端和服务器发送和接收那些空值的字段。 此外，在某些情况下，null可能是有意义的值 - 例如，JSON合并补丁RFC 7382）使用null来指示属性删除。

## [Should] 空数组不应该为 null
空数组可以表示为 []。

## [Should] 枚举应该被表示为字符串

