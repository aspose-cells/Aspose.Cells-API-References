---
title: "SheetSet 类"
linktitle: "SheetSet"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "SheetSet 类。封装了在 Go 中表示 sheetset 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/sheetset/
---

## SheetSet class

描述一组工作表。

```go

type SheetSet struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewSheetSet_int32Array](./newsheetset_int32array/) | 基于精确的工作表索引创建工作表集合。 |
| [NewSheetSet_stringArray](./newsheetset_stringarray/) | 基于精确的工作表名称创建工作表集合。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [SheetSet_GetActive](./sheetset_getactive/) | 获取包含工作簿中活动工作表的集合。 |
| [SheetSet_GetVisible](./sheetset_getvisible/) | 获取工作簿中可见工作表的集合，按原始顺序排列。 |
| [SheetSet_GetAll](./sheetset_getall/) | 获取工作簿中所有工作表的集合，按原始顺序排列。 |
