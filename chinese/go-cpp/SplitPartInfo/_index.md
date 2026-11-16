---
title: "SplitPartInfo 类"
linktitle: "SplitPartInfo"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "SplitPartInfo 类。封装在 Go 中表示 splitpartinfo 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/splitpartinfo/
---

## SplitPartInfo class

表示多个输入/输出中的单个输入/输出信息，例如在将电子表格转换为图像时要渲染的当前页。

```go

type SplitPartInfo struct  {
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
| [GetPartIndex](./getpartindex/) | 当前部分在序列中的索引（从 0 开始）。-1 表示没有多个部分，因此结果为单一。 |
| [GetSheetIndex](./getsheetindex/) | 当前部分所在工作表的索引。-1 表示只有一个工作表。 |
| [GetSheetName](./getsheetname/) | 当前部分所在工作表的名称。 |
