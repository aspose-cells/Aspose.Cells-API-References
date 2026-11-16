---
title: "PivotPageFields 类"
linktitle: "PivotPageFields"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "PivotPageFields 类。封装了在 Go 中表示 pivotpagefields 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/pivotpagefields/
---

## PivotPageFields class

表示当透视表数据源为合并范围时的透视页面项。它只能包含最多 4 项。

```go

type PivotPageFields struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewPivotPageFields](./newpivotpagefields/) | 表示透视表页面字段项。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [AddPageField](./addpagefield/) | 添加页面字段。 |
| [GetPageFieldCount](./getpagefieldcount/) | 获取页面字段的数量。 |
| [AddIdentify](./addidentify/) | 设置每个页面字段中用于标识数据范围的项标签。pageItemIndex.Length 必须等于 PageFieldCount，请先添加页面字段。 |
