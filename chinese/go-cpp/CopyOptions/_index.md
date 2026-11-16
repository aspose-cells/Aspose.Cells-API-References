---
title: "CopyOptions 类"
linktitle: "CopyOptions"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "CopyOptions 类。封装在 Go 中表示 copyoptions 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/copyoptions/
---

## CopyOptions class

表示复制选项。

```go

type CopyOptions struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewCopyOptions](./newcopyoptions/) | CopyOptions 构造函数。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetKeepMacros](./getkeepmacros/) | 指示是否保留宏； |
| [SetKeepMacros](./setkeepmacros/) | 指示是否保留宏； |
| [GetExtendToAdjacentRange](./getextendtoadjacentrange/) | 指示在将范围复制到相邻范围时是否扩展范围。 |
| [SetExtendToAdjacentRange](./setextendtoadjacentrange/) | 指示在将范围复制到相邻范围时是否扩展范围。 |
| [GetCopyNames](./getcopynames/) | 指示是否复制名称。 |
| [SetCopyNames](./setcopynames/) | 指示是否复制名称。 |
| [GetCopyInvalidFormulasAsValues](./getcopyinvalidformulasasvalues/) | 如果公式对目标位置无效，则仅复制数值。 |
| [SetCopyInvalidFormulasAsValues](./setcopyinvalidformulasasvalues/) | 如果公式对目标位置无效，则仅复制数值。 |
| [GetColumnCharacterWidth](./getcolumncharacterwidth/) | 指示是否以字符单位复制列宽。 |
| [SetColumnCharacterWidth](./setcolumncharacterwidth/) | 指示是否以字符单位复制列宽。 |
| [GetReferToSheetWithSameName](./getrefertosheetwithsamename/) | 在 Microsoft Excel 中，将引用其他工作表的公式复制到另一个工作表时，复制的公式应引用源工作簿。然而，在某些情况下，用户可能需要复制的公式引用同一工作簿中同名的工作表，例如这些工作表在此复制操作之前已经被复制，则此属性应保持为 true。 |
| [SetReferToSheetWithSameName](./setrefertosheetwithsamename/) | 在 Microsoft Excel 中，将引用其他工作表的公式复制到另一个工作表时，复制的公式应引用源工作簿。然而，在某些情况下，用户可能需要复制的公式引用同一工作簿中同名的工作表，例如这些工作表在此复制操作之前已经被复制，则此属性应保持为 true。 |
| [GetReferToDestinationSheet](./getrefertodestinationsheet/) | 在同一文件中复制范围且图表引用源工作表时，False 表示复制的图表数据源不会更改。True 表示复制的图表数据源引用目标工作表。 |
| [SetReferToDestinationSheet](./setrefertodestinationsheet/) | 在同一文件中复制范围且图表引用源工作表时，False 表示复制的图表数据源不会更改。True 表示复制的图表数据源引用目标工作表。 |
| [GetUpdateInvalidReferencesToTargetSheet](./getupdateinvalidreferencestotargetsheet/) | 指示如果未复制被引用的工作表，是否引用目标工作表。 |
| [SetUpdateInvalidReferencesToTargetSheet](./setupdateinvalidreferencestotargetsheet/) | 指示如果未复制被引用的工作表，是否引用目标工作表。 |
