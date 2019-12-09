# industrynav-api
> 产业导航API

	全局api格式：http://xxx:xxx/xxx

**状态码：**
> 1. 418:账号未登录
> 2. 404:404错误

- 描述：登录
- 地址：http://192.168.3.40:8910/toLogin
- 类型：POST
- 数据类型：application/json
- 请求头：xxx

- 请求体：
```javascript
	"username":"zhangsan"
	"password":"123456"
	
```
- 响应

```javascript
{
    "code": 1,       // 1:成功   0：失败
	"msg": "提示信息", 
	"data": [{
		"fieldA": "",  // xxx
		"fieldB": "    // xxx
	}]
}

```