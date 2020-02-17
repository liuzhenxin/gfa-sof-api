# 查询证书信任列表别名


> 总路径：/GFA_GM/v1_0/SOF

* 功能描述：查询证书信任列表别名。
* 演示地址：[localhost:8899/svs/GFA_GM/v1_0/SOF](localhost:8899/svs/GFA_GM/v1_0/SOF)
* 请求方式：`POST` [仅支持 POST]

* 请求参数 

* 字段说明

|字段|字段说明|字段类型|参数值|
|---|---|---|---|
|exec_name|方法名|String|SOF_getCertTrusthstAltNames|
|exec_args|参数|NULL|无|

``` json
{
    "exec_name":"SOF_getCertTrusthstAltNames",
    "exec_args":""
}
```

* 返回参数
>` 正常响应码:0,正常响应消息:SUCCESS `

``` json
{
  "code":"0",
  "msg":"SUCCESS"
  "data":"返回信任列表别名的组合,如: CAO01@CA002@CA003”
}
```

* 返回字段说明

|返回值字段|字段说明|字段类型|备注|
|---|---|---|---|
|status|状态码|String|0 表示请求成功，非0为错误码|
|msg|状态对应的信息|String|有成功失败等信息|
|data|证书信任列表别名|String|返回信任列表别名的组合,如: "CAO01@CA002@CA003”|








