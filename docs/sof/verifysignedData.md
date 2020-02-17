# 验证签名


> 总路径：/GFA_GM/v1_0/SOF

* 功能描述：验证数字签名。
* 演示地址：[localhost:8899/svs/GFA_GM/v1_0/SOF](localhost:8899/svs/GFA_GM/v1_0/SOF)
* 请求方式：`POST` [仅支持 POST]

* 请求参数 

* 字段说明

|字段|字段说明|字段类型|参数值|
|---|---|---|---|
|exec_name|方法名|String|SOF_verifySignedData|
|exec_args|参数|json|结构数据|
|base64EncodeCert|base64编码的数字证书|String|base64编码的字符串|
|inData|待验证的原文|String|待验证的原文|
|signValue|签名值|String|签名值,签名格式为数据类型A|


``` json
{
    "exec_name":"SOF_verifySignedData",
    "exec_args":{
        "base64EncodeCert":"base64编码的数字证书",
        "inData":"待验证的原文",
        "signValue":"签名值"
    }
}
```

* 返回参数
>` 正常响应码:0,正常响应消息:SUCCESS `

``` json
{
  "code":"0",
  "msg":"SUCCESS",
  "data":"true:验证成功 false:验证失败"
}
```

* 返回字段说明

|返回值字段|字段说明|字段类型|备注|
|---|---|---|---|
|status|状态码|String|0 表示请求成功，非0为错误码|
|msg|状态对应的信息|String|有成功失败等信息|
|data|验证结果|boolean|true 验证成功 false 验证失败|








