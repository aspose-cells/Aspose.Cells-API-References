---
title: "WebExtensionTaskPane 类"
linktitle: "WebExtensionTaskPane"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "WebExtensionTaskPane 类。封装在 Go 中表示 webextensiontaskpane 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/webextensiontaskpane/
---

## WebExtensionTaskPane class

表示持久化的任务窗格对象。

```go

type WebExtensionTaskPane struct  {
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
| [GetWebExtension](./getwebextension/) | 获取并设置与 taskpane 实例关联的 web extension 部分 |
| [SetWebExtension](./setwebextension/) | 获取并设置与 taskpane 实例关联的 web extension 部分 |
| [GetDockState](./getdockstate/) | 获取并设置此 taskpane 对象的上一次停靠位置。 |
| [SetDockState](./setdockstate/) | 获取并设置此 taskpane 对象的上一次停靠位置。 |
| [IsVisible](./isvisible/) | 指示文档打开时 Task Pane 是否默认显示为可见。 |
| [SetIsVisible](./setisvisible/) | 指示文档打开时 Task Pane 是否默认显示为可见。 |
| [IsLocked](./islocked/) | 指示 taskpane 在 UI 中是否锁定到文档，且用户无法关闭。 |
| [SetIsLocked](./setislocked/) | 指示 taskpane 在 UI 中是否锁定到文档，且用户无法关闭。 |
| [GetWidth](./getwidth/) | 获取并设置此 taskpane 实例的默认宽度值。 |
| [SetWidth](./setwidth/) | 获取并设置此 taskpane 实例的默认宽度值。 |
| [GetRow](./getrow/) | 获取并设置此 taskpane 在同一默认位置停靠的其他持久化 taskpane 中的索引（从外到内枚举）。 |
| [SetRow](./setrow/) | 获取并设置此 taskpane 在同一默认位置停靠的其他持久化 taskpane 中的索引（从外到内枚举）。 |
