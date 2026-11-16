---
title: "WebExtension 类"
linktitle: "WebExtension"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "WebExtension 类。封装在 Go 中表示 Web 扩展的对象。"
type: docs
weight: 200
url: /zh/go-cpp/webextension/
---

## WebExtension class

表示 Office 加载项实例。

```go

type WebExtension struct  {
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
| [GetId](./getid/) | 获取并设置唯一标识当前文档中 Office 加载项实例的标识。 |
| [SetId](./setid/) | 获取并设置唯一标识当前文档中 Office 加载项实例的标识。 |
| [IsFrozen](./isfrozen/) | 指示用户是否可以与 Office 加载项交互。 |
| [SetIsFrozen](./setisfrozen/) | 指示用户是否可以与 Office 加载项交互。 |
| [GetReference](./getreference/) | 获取对 Office 加载项的主要引用。 |
| [GetAlterReferences](./getalterreferences/) | 获取备用引用的列表。 |
| [GetProperties](./getproperties/) | 获取 Web 扩展的所有属性。 |
| [GetBindings](./getbindings/) | 获取 Office 加载项与文档中数据之间的所有绑定关系。 |
