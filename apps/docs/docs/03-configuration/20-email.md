---
slug: email
title: 配置邮件
---

# 配置邮件服务器

目前我们接入了第三方发件服务，需要自行注册后获取相关的 `id` 和 `secret`，并填入环境变量。

## Mailgun

### 注册 mailgun 并获取以下变量

API_KEY 可在账户中如下图位置找到：

![](img/mailgun-07.png)

| Mailgun 中的名称 | 填入环境变量的名称                | 例子               |
|--------------|--------------------------|------------------|
| 邮箱域名         | NEXT_PUBLIC_EMAIL_DOMAIN | mail.example.com |
| 访问密钥 ID      | EMAIL_API_KEY            | ffffffffffffffff |

### 新建邮件模版

![](img/mailgun-03.png)

选中模板样式：
![](img/mailgun-04.png)

确保 Name 填入 `verification_code` 无误
![](img/mailgun-05.png)

自行配置模版样式，确保在页面中通过花括号设置`name`和`code`变量，如图所示。

![](img/mailgun-06.png)

保存模版。
