---
title: "ListObject 类"
linktitle: "ListObject"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "ListObject 类。封装在 Go 中表示 listobject 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/listobject/
---

## ListObject class

表示工作表中的表。

```go

type ListObject struct  {
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
| [GetStartRow](./getstartrow/) | 获取范围的起始行。 |
| [GetStartColumn](./getstartcolumn/) | 获取范围的起始列。 |
| [GetEndRow](./getendrow/) | 获取范围的结束行。 |
| [GetEndColumn](./getendcolumn/) | 获取范围的结束列。 |
| [GetListColumns](./getlistcolumns/) | 获取此表的 ListColumn 列表。 |
| [Resize](./resize/) | 调整列表对象的范围。 |
| [PutCellValue_Int_Int_Object](./putcellvalue_int_int_object/) | 将值放入单元格。 |
| [PutCellValue_Int_Int_Object_Bool](./putcellvalue_int_int_object_bool/) | 将值放入单元格。 |
| [PutCellFormula_Int_Int_String](./putcellformula_int_int_string/) | 将公式放入表中的单元格。 |
| [PutCellFormula_Int_Int_String_Bool](./putcellformula_int_int_string_bool/) | 将公式放入表中的单元格。 |
| [GetShowHeaderRow](./getshowheaderrow/) | 获取和设置此 Table 是否显示标题行。 |
| [SetShowHeaderRow](./setshowheaderrow/) | 获取和设置此 Table 是否显示标题行。 |
| [GetShowTotals](./getshowtotals/) | 获取和设置此 TAble 是否显示汇总行。 |
| [SetShowTotals](./setshowtotals/) | 获取和设置此 TAble 是否显示汇总行。 |
| [GetDataRange](./getdatarange/) | 获取 Table 的数据范围。 |
| [UpdateColumnName](./updatecolumnname/) | 将所有列表列的名称更新到表中的单元格。 |
| [GetQueryTable](./getquerytable/) | 获取链接的 QueryTable。 |
| [GetDataSourceType](./getdatasourcetype/) | 获取表的数据源类型。 |
| [GetHasAutoFilter](./gethasautofilter/) | 指示是否已对该表应用自动筛选。 |
| [SetHasAutoFilter](./sethasautofilter/) | 指示是否已对该表应用自动筛选。 |
| [RemoveAutoFilter](./removeautofilter/) | 移除已对该表应用的自动筛选。 |
| [GetAutoFilter](./getautofilter/) | 获取该表的自动筛选。 |
| [GetDisplayName](./getdisplayname/) | 获取和设置表的显示名称。 |
| [SetDisplayName](./setdisplayname/) | 获取和设置表的显示名称。 |
| [GetComment](./getcomment/) | 获取和设置表的注释。 |
| [SetComment](./setcomment/) | 获取和设置表的注释。 |
| [GetShowTableStyleFirstColumn](./getshowtablestylefirstcolumn/) | 指示表中的第一列是否已应用样式。 |
| [SetShowTableStyleFirstColumn](./setshowtablestylefirstcolumn/) | 指示表中的第一列是否已应用样式。 |
| [GetShowTableStyleLastColumn](./getshowtablestylelastcolumn/) | 指示表中的最后一列是否已应用样式。 |
| [SetShowTableStyleLastColumn](./setshowtablestylelastcolumn/) | 指示表中的最后一列是否已应用样式。 |
| [GetShowTableStyleRowStripes](./getshowtablestylerowstripes/) | 指示是否已对行条纹格式化。 |
| [SetShowTableStyleRowStripes](./setshowtablestylerowstripes/) | 指示是否已对行条纹格式化。 |
| [GetShowTableStyleColumnStripes](./getshowtablestylecolumnstripes/) | 指示是否已对列条纹格式化。 |
| [SetShowTableStyleColumnStripes](./setshowtablestylecolumnstripes/) | 指示是否已对列条纹格式化。 |
| [ApplyStyleToRange](./applystyletorange/) | 将表样式应用于范围。 |
| [ConvertToRange](./converttorange/) | 将表转换为范围。 |
| [ConvertToRange_TableToRangeOptions](./converttorange_tabletorangeoptions/) | 将表转换为范围。 |
| [GetTableStyleType](./gettablestyletype/) | 获取内置的表样式。 |
| [SetTableStyleType](./settablestyletype/) | 获取内置的表样式。 |
| [GetTableStyleName](./gettablestylename/) | 获取和设置表样式名称。 |
| [SetTableStyleName](./settablestylename/) | 获取和设置表样式名称。 |
| [GetXmlMap](./getxmlmap/) | 获取用于此列表的 XmlMap。 |
| [GetAlternativeText](./getalternativetext/) | 获取和设置替代文本。 |
| [SetAlternativeText](./setalternativetext/) | 获取和设置替代文本。 |
| [GetAlternativeDescription](./getalternativedescription/) | 获取并设置备用描述。 |
| [SetAlternativeDescription](./setalternativedescription/) | 获取并设置备用描述。 |
