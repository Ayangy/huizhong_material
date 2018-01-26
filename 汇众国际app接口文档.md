# 汇众国际app接口文档

原型图地址: https://eocn8n.axshare.com

## 1、用户

### 1.1、注册

服务地址：/app/consumer/register

请求方法：POST

请求body：

### 1.2、用户登录

服务地址：/app/consumer/login

请求方法：GET

请求参数：

| 参数           | 类型     | 是否必须 | 默认值  | 说明   |
| ------------ | ------ | ---- | ---- | ---- |
| mobileNumber | int    | 是    |      | 手机号  |
| pwd          | String | 是    |      | 用户密码 |

### 1.3、修改密码

服务地址：/app/consumer/changePwd

请求方法：GET

请求参数：

| 参数           | 类型   | 是否必须 | 默认值  | 说明   |
| ------------ | ---- | ---- | ---- | ---- |
| mobileNumber | int  | 是    |      | 手机号  |
| authCode     | int  | 是    |      | 验证码  |
| newPwd       | int  | 是    |      | 新密码  |



## 2、首页

### 2.1、获取banner图

服务地址：/app/homePage/getBannerImg

请求方法：GET

请求参数：

### 2.2、获取商家列表

服务地址：/app/homePage/getMerchantList

请求方法：GET

请求参数：

| 参数    | 类型   | 是否必须 | 默认值  | 说明   |
| ----- | ---- | ---- | ---- | ---- |
| index | int  | 否    | 1    | 第几页  |
| size  | int  | 否    | 6    | 每页几条 |

### 2.3、获取商家详情

服务地址：/app/homePage/getMerchantDetail

请求方法：GET

请求参数：

| 参数         | 类型   | 是否必须 | 默认值  | 说明   |
| ---------- | ---- | ---- | ---- | ---- |
| merchantId | int  | 是    |      | 商家id |

## 3、消费金

### 3.1、