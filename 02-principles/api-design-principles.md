# API 设计原则

比较SOAP和REST的SOA Web服务接口风格，前者倾向于围绕用例特定和专用的操作。相比之下，REST集中在业务（数据）实体上，这些实体暴露为通过URI标识的资源，并且可以通过使用不同表示，自描述消息和超媒体的标准化CRUD方法来操作。 REST风格的API往往不是特定于用例，并且与客户端/服务器之间的耦合度较低，更适合作为平台接口，用于不同的客户端应用程序。

- 我们更喜欢 REST-based APIs with JSON payloads
- 我们更喜欢系统是真正的 RESTful （REST API 成熟度级别2）

![](/assets/restful maturity level.png)

RESTful API 设计和使用的一条重要原则是伯斯塔尔法则（Postel's Law）， 也称为健壮性原则：接收时要开放自由；发送时要保守。
    



