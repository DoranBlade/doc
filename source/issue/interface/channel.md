title: 渠道信息
---
### 渠道推送接口
##### 接口描述
+ 分发渠道推送自有的渠道信息到平台，接口支持批量推送
+ 接口方法
> post

+ 接口地址
>http://${host}/channel/insert
host依环境而定

##### 参数描述
+ 总体参数

|参数名|类型|是否必要|说明|
|--|--|--|--|
|requestNo|String|是|请求的唯一标识符|
|userName|String|是|分发渠道用户名, 由悦保提供|
|password|String|是|分发渠道密码, 由悦保提供|
|data|List&lt;Channel>|是|推送的数据,以数组形式|

+ Channel参数

|参数名|类型|是否必要|说明|
|--|--|--|--|
|code|String|是|渠道编码|
|names|String|是|渠道名称|
|companyCode|String|是|渠道所属分公司|


##### 报文示例

``` json
{
    "requestNo": "jsdfoiajeoijafsoijfoajef",
    "userName": "test",
    "password": "test",
    "data": [
        {
            
        }
    ]
}
```