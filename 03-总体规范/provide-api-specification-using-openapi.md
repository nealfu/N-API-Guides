# Must:Provide API Specification using OpenAPI 
我们使用 OpenAPI 规范（又名 Swagger 规范）作为标准来定义 API 规格说明文件。API 设计者必须使用 YAML 来提供 API 规格说明文件来提高可读性。为方便 API 管理，API 规格说明必须包含以下元信息：

- \#/info/title （API 唯一标识）
- \#/info/version    （API 规格说明的版本号）
- \#/info/description    （包含对 API 的正确描述）
- \#/info/contact/{name, url, email}    (包含此 API 的负责团队的信息)

OpenAPI 规范请参考 [OpenAPI 3.0](https://swagger.io/specification/)。

API 规格文件应该使用Git做好版本控制，最好和实现它的代码放一起。
