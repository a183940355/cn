# deleteAliasIp


## 描述
删除别名IP

## 请求方式
DELETE

## 请求地址
https://edcps.jdcloud-api.com/v1/regions/{regionId}/aliasIps/{aliasIpId}

|名称|类型|是否必需|默认值|描述|
|---|---|---|---|---|
|**regionId**|String|True| |地域ID，可调用接口（describeEdCPSRegions）获取分布式云物理服务器支持的地域|
|**aliasIpId**|String|True| |别名IP ID|

## 请求参数
|名称|类型|是否必需|默认值|描述|
|---|---|---|---|---|
|**clientToken**|String|False| |由客户端生成，用于保证请求的幂等性，长度不能超过36个字符；<br/><br>如果多个请求使用了相同的clientToken，只会执行第一个请求，之后的请求直接返回第一个请求的结果<br/><br>|


## 返回参数
|名称|类型|描述|
|---|---|---|
|**result**|[Result](#Result)| |
|**requestId**|String| |

### <a name="Result">Result</a>
|名称|类型|描述|
|---|---|---|
|**success**|Boolean|删除操作是否成功|

## 返回码
|返回码|描述|
|---|---|
|**200**|OK|
|**400**|Bad request|
|**404**|Not found|
|**500**|Internal server error|
|**503**|Service unavailable|