---
title: "DeleteBlankOptions 类"
linktitle: "DeleteBlankOptions"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "DeleteBlankOptions 类。封装了在 Go 中表示 deleteblankoptions 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/deleteblankoptions/
---

## DeleteBlankOptions class

表示删除空单元格/行/列的设置。

```go

type DeleteBlankOptions struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewDeleteBlankOptions](./newdeleteblankoptions/) | 默认构造函数。 |
| [NewDeleteBlankOptions_DeleteOptions](./newdeleteblankoptions_deleteoptions/) | 从父对象构造。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetEmptyStringAsBlank](./getemptystringasblank/) | 指示当单元格的值为空字符串时是否将其视为空白。默认值为 true。 |
| [SetEmptyStringAsBlank](./setemptystringasblank/) | 指示当单元格的值为空字符串时是否将其视为空白。默认值为 true。 |
| [GetEmptyFormulaValueAsBlank](./getemptyformulavalueasblank/) | 指示当单元格是公式且计算结果为 null 或空字符串时是否将其视为空白。默认值为 false。 |
| [SetEmptyFormulaValueAsBlank](./setemptyformulavalueasblank/) | 指示当单元格是公式且计算结果为 null 或空字符串时是否将其视为空白。默认值为 false。 |
| [GetDrawingsAsBlank](./getdrawingsasblank/) | 指示诸如图片、形状、图表等绘图相关对象是否将被视为空白。默认值为 true。 |
| [SetDrawingsAsBlank](./setdrawingsasblank/) | 指示诸如图片、形状、图表等绘图相关对象是否将被视为空白。默认值为 true。 |
| [GetMergedCellsShrinkType](./getmergedcellsshrinktype/) | 指示在删除空白行/列时如何处理合并单元格。 |
| [SetMergedCellsShrinkType](./setmergedcellsshrinktype/) | 指示在删除空白行/列时如何处理合并单元格。 |
| [GetStartIndex](./getstartindex/) | 指定要检查并删除空行/列的范围的起始行/列索引。 |
| [SetStartIndex](./setstartindex/) | 指定要检查并删除空行/列的范围的起始行/列索引。 |
| [GetEndIndex](./getendindex/) | 指定要检查并删除空行/列的范围的结束行/列索引（含）。默认值为 -1，-1 表示需要检查的所有对象（单元格、图形等）的最大范围。 |
| [SetEndIndex](./setendindex/) | 指定要检查并删除空行/列的范围的结束行/列索引（含）。默认值为 -1，-1 表示需要检查的所有对象（单元格、图形等）的最大范围。 |
| [GetUpdateReference](./getupdatereference/) | 指示是否在其他工作表中更新引用。 |
| [SetUpdateReference](./setupdatereference/) | 指示是否在其他工作表中更新引用。 |
| [GetFormulaChangeMonitor](./getformulachangemonitor/) | 获取/设置用于跟踪删除导致的更改的监视器。 |
| [SetFormulaChangeMonitor](./setformulachangemonitor/) | 获取/设置用于跟踪删除导致的更改的监视器。 |
