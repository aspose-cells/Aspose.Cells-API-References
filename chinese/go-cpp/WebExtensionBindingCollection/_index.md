---
title: "WebExtensionBindingCollection 类"
linktitle: "WebExtensionBindingCollection"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "WebExtensionBindingCollection 类。封装表示 Go 中 webextensionbindingcollection 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/webextensionbindingcollection/
---

## WebExtensionBindingCollection class

表示 Office 加载项与文档中数据之间的绑定关系列表。

```go

type WebExtensionBindingCollection struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewWebExtensionBindingCollection](./newwebextensionbindingcollection/) | 默认构造函数。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [Get](./get/) | 通过特定索引获取 web extension 绑定关系。 |
| [Add](./add/) | 在 Office Add-in 与文档中的数据之间添加绑定关系。 |
| [GetCount](./getcount/) | 获取实例中包含的元素数量。 |
