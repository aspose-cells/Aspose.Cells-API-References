---
title: "PasteOptions 类"
linktitle: "PasteOptions"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "PasteOptions 类。封装了在 Go 中表示 pasteoptions 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/pasteoptions/
---

## PasteOptions class

表示粘贴特殊选项。

```go

type PasteOptions struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewPasteOptions](./newpasteoptions/) | 默认构造函数。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetPasteType](./getpastetype/) | 粘贴特殊类型。 |
| [SetPasteType](./setpastetype/) | 粘贴特殊类型。 |
| [GetShiftFormulasOfShapes](./getshiftformulasofshapes/) | 指示在复制范围时是否移动形状的公式。 |
| [SetShiftFormulasOfShapes](./setshiftformulasofshapes/) | 指示在复制范围时是否移动形状的公式。 |
| [GetSkipBlanks](./getskipblanks/) | 指示是否跳过空单元格。 |
| [SetSkipBlanks](./setskipblanks/) | 指示是否跳过空单元格。 |
| [GetKeepOldTables](./getkeepoldtables/) | 在目标范围内保留表格。 |
| [SetKeepOldTables](./setkeepoldtables/) | 在目标范围内保留表格。 |
| [GetOnlyVisibleCells](./getonlyvisiblecells/) | True 表示仅复制可见单元格。 |
| [SetOnlyVisibleCells](./setonlyvisiblecells/) | True 表示仅复制可见单元格。 |
| [GetTranspose](./gettranspose/) | True 表示在粘贴范围时转置行和列。默认值为 False。 |
| [SetTranspose](./settranspose/) | True 表示在粘贴范围时转置行和列。默认值为 False。 |
| [GetOperationType](./getoperationtype/) | 获取和设置粘贴范围时的操作类型。 |
| [SetOperationType](./setoperationtype/) | 获取和设置粘贴范围时的操作类型。 |
| [GetIgnoreLinksToOriginalFile](./getignorelinkstooriginalfile/) | 忽略指向原始文件的链接。 |
| [SetIgnoreLinksToOriginalFile](./setignorelinkstooriginalfile/) | 忽略指向原始文件的链接。 |
