---
title: provider_id 属性
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 70
url: /zh/python-net/aspose.cells.digitalsignatures/digitalsignature/provider_id/
is_root: false
---
## provider_id 属性

指定签名提供者的类 ID。
默认值为空（全为零）Guid。

### 评论

密码服务提供程序 (CSP) 是一个独立的软件模块，它实际执行用于身份验证、编码和加密的密码算法。
Microsoft Office 为其默认签名提供程序保留值 {00000000-0000-0000-0000-000000000000}，
和 {000CD6A4-0000-0000-C000-000000000046} 为其东亚签名提供商。

额外安装的提供程序的 GUID 应从提供程序随附的文档中获取。
### 定义：
```python
@property
def provider_id(self):
    ...
@provider_id.setter
def provider_id(self, value):
    ...
```

### 也可以看看
* 模块 [aspose.cells.digitalsignatures](../../)
* 类 [DigitalSignature](/cells/zh/python-net/aspose.cells.digitalsignatures/digitalsignature)
