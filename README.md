# Get-MQ-Message-From-Ctwing
从Ctwing物联网平台获取MQ消息推送

代码第28行
raw_info = apis.aep_device_status.QueryDeviceStatusList('', '', '{"productId":"","deviceId":""}')
缺少的四个参数分别为Ctwing平台的应用 App Key、App Secret、产品ID和设备ID，需正确填写之后才能正常获取信息！
