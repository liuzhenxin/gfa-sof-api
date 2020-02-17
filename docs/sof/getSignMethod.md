# 获得当前签名算法


> 总路径：/GFA_GM/v1_0/SOF

* 功能描述：获得当前签名算法。
* 演示地址：[localhost:8899/svs/GFA_GM/v1_0/SOF](localhost:8899/svs/GFA_GM/v1_0/SOF)
* 请求方式：`POST` [仅支持 POST]

* 请求参数 

* 字段说明

|字段|字段说明|字段类型|参数值|
|---|---|---|---|
|exec_name|方法名|String|SOF_getSignMethod|
|exec_args|参数|NULL|无|

``` json
{
    "exec_name":"SOF_getSignMethod",
    "exec_args":""
}
```

* 返回参数
>` 正常响应码:0,正常响应消息:SUCCESS `

``` json
{
  "code":"0",
  "msg":"SUCCESS",
  "data":"当前的签名算法标识（详见GM/T0006)"
}
```

* 返回字段说明

|返回值字段|字段说明|字段类型|备注|
|---|---|---|---|
|status|状态码|String|0 表示请求成功，非0为错误码|
|msg|状态对应的信息|String|有成功失败等信息|
|data|当前的签名算法标识|long|当前的签名算法标识（详见GM/T0006)|








