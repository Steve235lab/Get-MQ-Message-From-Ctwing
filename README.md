# Get-MQ-Message-From-Ctwing
从Ctwing物联网平台获取MQ消息推送

使用了Ctwing平台提供的SDK，适用于Windows平台。
使用前需在Ctwing平台完成账号注册并添加产品-设备并创建一个“第三方应用”，更多信息请查阅相关开发手册。

*****
get_device_statics.py 是数据接收及处理储存程序，由Steve编写
第25行
raw_info = apis.aep_device_status.QueryDeviceStatusList('', '', '{"productId":"","deviceId":""}')
缺少的四个参数分别为Ctwing平台的应用 App Key、App Secret、产品ID和设备ID，需正确填写之后才能正常获取信息！
*****

*****
aep_device_status.py 包含该程序所需的api函数，由Ctwing平台提供。
*****
