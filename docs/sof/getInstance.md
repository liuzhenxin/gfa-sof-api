# 设置证书信任列表


> 总路径：/GFA_GM/v1_0/SOF

* 功能描述：初始化接口,通过应用别名获取实例,应用别名关联所配置的证书、密钥、信任证书链、算法类型、CRL及证书验证策略等。用户如果有多应用需求,可同时获取多个实例对象满足不同的使用需求,不同的实例在调用方法时会有不同效果(如:不同密钥的签名,不同算法的加密,不同的证书验证策略)。
* 演示地址：[localhost:8899/svs/GFA_GM/v1_0/SOF](localhost:8899/svs/GFA_GM/v1_0/SOF)
* 请求方式：`POST` [仅支持 POST]

* 请求参数

* 字段说明

|字段|字段说明|字段类型|参数值|
|---|---|---|---|
|exec_name|方法名|String|SOF_getInstance|
|exec_args|参数|json|结构数据|
|ctlAltName|证书信任列表别名|String|示例：test_ca|

``` json
{
    "exec_name":"SOF_getInstance",
    "exec_args":{
        "appName":"应用名称"
    }
}
```

* 返回参数
>` 正常响应码:0,正常响应消息:SUCCESS `

``` json
{
  "code":"0",
  "msg":"SUCCESS",
  "data":{
            "appID":"应用ID",
            "appName":"应用名称"
            "appIP":"应用IP"
         }
}
```

* 返回字段说明

|返回值字段|字段说明|字段类型|备注|
|---|---|---|---|
|status|状态码|String|0 表示请求成功，非0为错误码|
|msg|状态对应的信息|String|有成功失败等信息|
|data|应用名称对应的实例|String|返回此应用策略名称所对应的实例|








