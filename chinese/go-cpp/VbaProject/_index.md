---
title: "VbaProject 类"
linktitle: "VbaProject"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "VbaProject 类。封装在 Go 中表示 vbaproject 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/vbaproject/
---

## VbaProject class

表示 VBA 项目。

```go

type VbaProject struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [Sign](./sign/) | 使用 DigitalSignature 对此 VBA 项目进行签名 |
| [IsValidSigned](./isvalidsigned/) | 指示 VBA 项目的签名是否有效。 |
| [GetCertRawData](./getcertrawdata/) | 如果此 VBA 项目已签名，则获取证书原始数据。 |
| [GetEncoding](./getencoding/) | 获取并设置 VBA 项目的编码。 |
| [SetEncoding](./setencoding/) | 获取并设置 VBA 项目的编码。 |
| [GetName](./getname/) | 获取并设置 VBA 项目的名称。 |
| [SetName](./setname/) | 获取并设置 VBA 项目的名称。 |
| [IsSigned](./issigned/) | 指示 VBAcode 是否已签名。 |
| [Protect](./protect/) | 保护或取消保护此 VBA 项目。 |
| [IsProtected](./isprotected/) | 指示此 VBA 项目是否受保护。 |
| [IsLockedForView](./islockedforview/) | 指示此 VBA 项目是否被锁定以供查看。如果为 true，代码将不可见。 |
| [Copy](./copy/) | 从其他文件复制 VBA 项目。 |
| [GetModules](./getmodules/) | 获取所有 VbaModule 对象。 |
| [GetReferences](./getreferences/) | 获取 VBA 项目的所有引用。 |
| [ValidatePassword](./validatepassword/) | 验证保护密码。 |
