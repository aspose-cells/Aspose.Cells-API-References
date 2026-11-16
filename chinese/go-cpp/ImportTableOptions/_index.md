---
title: "ImportTableOptions 类"
linktitle: "ImportTableOptions"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "ImportTableOptions 类。封装了在 Go 中表示 importtableoptions 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/importtableoptions/
---

## ImportTableOptions class

表示将数据导入单元格的选项。

```go

type ImportTableOptions struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewImportTableOptions](./newimporttableoptions/) | 创建默认的导入选项。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetConvertGridStyle](./getconvertgridstyle/) | 指示是否将网格视图的样式应用于单元格。 |
| [SetConvertGridStyle](./setconvertgridstyle/) | 指示是否将网格视图的样式应用于单元格。 |
| [GetConvertNumericData](./getconvertnumericdata/) | 获取或设置一个值，该值指示是否应将字符串值转换为数值或日期值。 |
| [SetConvertNumericData](./setconvertnumericdata/) | 获取或设置一个值，该值指示是否应将字符串值转换为数值或日期值。 |
| [GetInsertRows](./getinsertrows/) | 指示是否应为导入的数据记录添加新行。 |
| [SetInsertRows](./setinsertrows/) | 指示是否应为导入的数据记录添加新行。 |
| [GetShiftFirstRowDown](./getshiftfirstrowdown/) | 指示在插入行时是否将第一行向下移动。 |
| [SetShiftFirstRowDown](./setshiftfirstrowdown/) | 指示在插入行时是否将第一行向下移动。 |
| [IsFieldNameShown](./isfieldnameshown/) | 指示是否应导入字段名称。 |
| [SetIsFieldNameShown](./setisfieldnameshown/) | 指示是否应导入字段名称。 |
| [GetExportCaptionAsFieldName](./getexportcaptionasfieldname/) | 指示是否将标题导出为字段名称 |
| [SetExportCaptionAsFieldName](./setexportcaptionasfieldname/) | 指示是否将标题导出为字段名称 |
| [GetDateFormat](./getdateformat/) | 获取或设置导入的日期时间值单元格的日期格式字符串。 |
| [SetDateFormat](./setdateformat/) | 获取或设置导入的日期时间值单元格的日期格式字符串。 |
| [GetNumberFormats](./getnumberformats/) | 获取或设置数字格式 |
| [SetNumberFormats](./setnumberformats/) | 获取或设置数字格式 |
| [GetStyles](./getstyles/) | 获取并设置表格每列的样式。 |
| [SetStyles](./setstyles/) | 获取并设置表格每列的样式。 |
| [GetIsFormulas](./getisformulas/) | 指示数据是否为公式。 |
| [SetIsFormulas](./setisformulas/) | 指示数据是否为公式。 |
| [GetTotalRows](./gettotalrows/) | 获取或设置要从数据源导入的总行数。-1 表示导入给定数据源的所有行。 |
| [SetTotalRows](./settotalrows/) | 获取或设置要从数据源导入的总行数。-1 表示导入给定数据源的所有行。 |
| [GetTotalColumns](./gettotalcolumns/) | 获取或设置要从数据源导入的总列数。-1 表示导入给定数据源的所有列。 |
| [SetTotalColumns](./settotalcolumns/) | 获取或设置要从数据源导入的总列数。-1 表示导入给定数据源的所有列。 |
| [GetColumnIndexes](./getcolumnindexes/) | 获取或设置要从数据源导入的列（基于 0 的索引）。null 表示应导入所有列。 |
| [SetColumnIndexes](./setcolumnindexes/) | 获取或设置要从数据源导入的列（基于 0 的索引）。null 表示应导入所有列。 |
| [GetDefaultValues](./getdefaultvalues/) | 表格中值的默认值为 null。 |
| [SetDefaultValues](./setdefaultvalues/) | 表格中值的默认值为 null。 |
| [IsHtmlString](./ishtmlstring/) | 指示该值是否包含 HTML 标签。 |
| [SetIsHtmlString](./setishtmlstring/) | 指示该值是否包含 HTML 标签。 |
| [GetCheckMergedCells](./getcheckmergedcells/) | 指示是否检查合并单元格。 |
| [SetCheckMergedCells](./setcheckmergedcells/) | 指示是否检查合并单元格。 |
