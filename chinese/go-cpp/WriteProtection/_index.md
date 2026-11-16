---
title: "WriteProtection 类"
linktitle: "WriteProtection"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "WriteProtection 类。封装了在 Go 中表示 writeprotection 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/writeprotection/
---

## WriteProtection class

指定工作簿的写保护设置。

```go

type WriteProtection struct  {
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
| [GetAuthor](./getauthor/) | 获取和设置作者。 |
| [SetAuthor](./setauthor/) | 获取和设置作者。 |
| [GetRecommendReadOnly](./getrecommendreadonly/) | 指示是否选择了“建议只读”选项。 |
| [SetRecommendReadOnly](./setrecommendreadonly/) | 指示是否选择了“建议只读”选项。 |
| [IsWriteProtected](./iswriteprotected/) | 指示此工作簿是否受写保护。 |
| [GetPassword](./getpassword/) | 设置用于修改文件的受保护密码。 |
| [SetPassword](./setpassword/) | 设置用于修改文件的受保护密码。 |
| [ValidatePassword](./validatepassword/) | 如果指定的密码与文件受写保护时使用的密码相同，则返回 true。 |
