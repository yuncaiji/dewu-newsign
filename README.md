
# 引流
## 得物App newSign逆向过程
## 搜索关键词newSign
## 得物app的newSign签名
## 毒APP newSign算法分析 得物逆向分析
## 得物app的newSign签名
## 得物newsign API


# 请求说明
本平台 API 不完全要求遵循 REST 标准进行设计。
所有请求和响应的编码均为 UTF-8。
所有的请求方式（Method）如无特殊说明均为 GET 请求方式
所有请求都有权限验证，都需要传入token 进行验证。获取token请联系：添加好友时请备注:api
![微信](weixin.jpg)


# 使用建议
由于接口调用有时候会遇到失败或者不稳定的场景，接口对接建议如下：

接口超时时间建议设置为10秒，如果超时时间设置太短，偶尔会触发风控，响应不及时
当接口返回code字段为0时表示请求成功，如果资源不存在重试后还是返回0 或者数据有问题，可以联系我们反馈修复，且会补偿次数
对于重试请求，建议中间sleep 1-3秒，也可以设置一个最大重试次数


# 返回信息说明
如上，通过返回结果，如果返回 code 为0 就会扣费。
请求错误模板，请求错误不会增加计数（不会扣费），如果偶尔出现错误，重试就行。连续错误，联系管理员。
```
{
    'code': -1,
    'msg': 'error'
}
```


