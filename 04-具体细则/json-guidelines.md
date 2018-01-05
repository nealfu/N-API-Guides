## [Should] 数组名称应该为复数
为了表明它们包含多个值，应该复数化数组名称。 这意味着对象名称应该是单数。

## [Must] 布尔属性值不能为空
JSON属性不得显示为空值。 一个布尔值本质上是一个封闭的枚举值，true和false。 如果内容具有有意义的空值，则强烈倾向于用枚举的命名值或状态来替换布尔值 - 例如用true或false接受的_terms_and_conditions可以用具有值yes，no和unknown的terms_and_conditions替换。