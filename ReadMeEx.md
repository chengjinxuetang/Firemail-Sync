# Firemail-Sync
open sourece mail client refer to MailSpring

编译条件

支持VS2017













安装
VS2015
VS2013

下载源码后，打开

Firemail-Sync\Windows\mailsync.sln

如下图

![image](https://github.com/chengjinxuetang/Firemail-Sync/blob/main/Pictures/sps1.png)

这里不要升级,即点取消

打开成功后，如下图：

![image](https://github.com/chengjinxuetang/Firemail-Sync/blob/main/Pictures/sps2.png)

即：libetpan和mailsync使用VS2015编译，而mailcore2使用VS2013编译



C:\Users\Administrator\AppData\Roaming\Firemail-dev

_putenv("CONFIG_DIR_PATH=C:\\Users\\Administrator\\AppData\\Roaming\\Firemail-dev");
//_putenv("IDENTITY_SERVER=https://id.firemail.wang");
_putenv("IDENTITY_SERVER=unknown");
firemail\app\mailsync --mode migrate




--identity "{\"id\":\"2137538a-6cb1-4c1f-b593-deb6103cf88b\",\"firstName\":\"Test\",\"lastName\":\"User\",\"emailAddress\":\"testuser@getmailspring.com\",\"object\":\"identity\",\"createdAt\":\"2017-09-27T19:41:39.000Z\",\"stripePlan\":\"Basic\",\"stripePlanEffective\":\"Basic\",\"stripeCustomerId\":\"XXXXX\",\"stripePeriodEnd\":\"2017-10-27T19:41:39.000Z\",\"featureUsage\":{\"snooze\":{\"quota\":15,\"period\":\"weekly\",\"usedInPeriod\":0,\"featureLimitName\":\"basic-limit\"},\"send-later\":{\"quota\":10,\"period\":\"weekly\",\"usedInPeriod\":2,\"featureLimitName\":\"basic-limit\"},\"send-reminders\":{\"quota\":10,\"period\":\"weekly\",\"usedInPeriod\":2,\"featureLimitName\":\"basic-limit\"}},\"token\":\"b7670d34-d4d4-4391-9757-a8d37f31f839\"}" --account "<your account object with .settings populated>" --mode sync

--mode migrate


--account "{\\"id\":\"9227059b\",\"metadata\":[],\"name\":\"15313159857\",\"provider\":\"imap\",\"emailAddress\":\"15313159857@163.com\",\"settings\":{\"imap_host\":\"imap.163.com\",\"imap_port\":993,\"imap_username\":\"15313159857@163.com\",\"imap_security\":\"SSL / TLS\",\"imap_allow_insecure_ssl\":false,\"smtp_host\":\"smtp.163.com\",\"smtp_port\":465,\"smtp_username\":\"15313159857@163.com\",\"smtp_security\":\"SSL / TLS\",\"smtp_allow_insecure_ssl\":false},\"label\":\"15313159857@163.com\",\"autoaddress\":{\"type\":\"bcc\",\"value\":\"\"},\"aliases\":[],\"syncState\":\"ok\",\"syncError\":null,\"authedAt\":1632233127.507,\"color\":\"\",\"__cls\":\"Account\"}" --mode sync
