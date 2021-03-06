
> ios快捷指令本质是HTTP API 发布消息的实际运用，以下是几个极简的快捷指令编写案例

## 发送命令字段

 1. 网页 -> **获取URL内容**<br />
   在URL中填入<br />
     `https://api.cooleiot.tech/mqtt/publish?key={APIKEY}`<br />
     请注意将上面的`{APIKEY}`填为设备API密钥<br />
     方法为`POST`<br />
     请求体为`JSON`，添加新字段选择**文本**<br />
     输入键为`command`，值为您想要发送的命令字段
 2. 脚本 -> **从输入中获取词典**<br />
   会自动添加**URL的内容**，即显示`从URL的内容获取词典`
 3. 脚本 -> **获取词典值**<br />
   只需手动输入`msg`，即显示`在词典中获取msg的值`
 4. 脚本 -> **显示提醒**<br />
   点击原来的“**是否继续**”，选择变量替换为`词典值`<br />
     可自定义标题，如：执行结果<br />
     将`显示取消按钮`关闭勾选

## 运行场景

 1. 网页 -> **获取URL内容**<br />
   在URL中填入<br />
    `https://api.cooleiot.tech/mqtt/runscene?key={APIKEY}`<br />
     请注意将上面的`{APIKEY}`填为场景API密钥<br />
     方法为`POST`<br />
 2. 脚本 -> **从输入中获取词典**<br />
   会自动添加**URL的内容**，即显示`从URL的内容获取词典`
 3. 脚本 -> **获取词典值**<br />
   只需手动输入`msg`，即显示`在词典中获取msg的值`
 4. 脚本 -> **显示提醒**<br />
   点击原来的“**是否继续**”，选择变量替换为`词典值`<br />
     可自定义标题，如：执行结果<br />
     将`显示取消按钮`关闭勾选