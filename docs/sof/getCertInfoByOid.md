# 获得证书扩展信息


> 总路径：/GFA_GM/v1_0/SOF

* 功能描述：根据OID获取证书扩展信息。
* 演示地址：[localhost:8899/svs/GFA_GM/v1_0/SOF](localhost:8899/svs/GFA_GM/v1_0/SOF)
* 请求方式：`POST` [仅支持 POST]

* 请求参数 

* 字段说明

|字段|字段说明|字段类型|参数值|
|---|---|---|---|
|exec_name|方法名|String|SOF_getCertInfoByOid|
|exec_args|参数|json|结构数据|
|base64EncodeCert|base64编码的数字证书|String|base64编码的字符串|
|oid|私有扩展对象ID|String|私有扩展对象ID,如："1.2.156.10197.***"|


``` json
{
    "exec_name":"SOF_getCertInfoByOid",
    "exec_args":{
        "base64EncodeCert":"base64编码的数字证书",
        "oid":"获取证书信息的类型"
    }
}
```

* 返回参数
>` 正常响应码:0,正常响应消息:SUCCESS `

``` json
{
  "code":"0",
  "msg":"SUCCESS",
  "data":"证书OID对应的信息"
}
```

* 返回字段说明

|返回值字段|字段说明|字段类型|备注|
|---|---|---|---|
|status|状态码|String|0 表示请求成功，非0为错误码|
|msg|状态对应的信息|String|有成功失败等信息|
|data|证书OID对应的信息|String|证书OID对应的信息|








