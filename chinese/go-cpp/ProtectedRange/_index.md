---
title: "ProtectedRange 类"
linktitle: "ProtectedRange"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "ProtectedRange 类。封装在 Go 中表示 protectedrange 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/protectedrange/
---

## ProtectedRange class

在工作表保护开启时，允许编辑的指定范围。

```go

type ProtectedRange struct  {
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
| [GetName](./getname/) | 获取范围标题。这用作描述符，而不是命名范围定义。 |
| [SetName](./setname/) | 获取范围标题。这用作描述符，而不是命名范围定义。 |
| [GetCellArea](./getcellarea/) | 获取表示要受保护的单元格区域的 CellArea 对象。 |
| [GetAreas](./getareas/) | 获取所有引用的区域。 |
| [AddArea](./addarea/) | 向此添加一个引用的区域。 |
| [IsProtectedWithPassword](./isprotectedwithpassword/) | 指示工作表是否已使用密码受保护。 |
| [GetPassword](./getpassword/) | 表示用于保护该范围的密码。 |
| [SetPassword](./setpassword/) | 表示用于保护该范围的密码。 |
| [GetSecurityDescriptor](./getsecuritydescriptor/) | 安全描述符定义了可以在不提供密码的情况下编辑此范围的用户帐户。 |
| [SetSecurityDescriptor](./setsecuritydescriptor/) | 安全描述符定义了可以在不提供密码的情况下编辑此范围的用户帐户。 |
