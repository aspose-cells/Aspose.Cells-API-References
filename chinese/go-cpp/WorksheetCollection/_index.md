---
title: "WorksheetCollection 类"
linktitle: "WorksheetCollection"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "WorksheetCollection 类。封装了在 Go 中表示 worksheetcollection 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/worksheetcollection/
---

## WorksheetCollection class

封装 <see cref=\"Worksheet\"/> 对象的集合。

```go

type WorksheetCollection struct  {
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
| [GetWebExtensionTaskPanes](./getwebextensiontaskpanes/) | 获取任务窗格的列表。 |
| [GetWebExtensions](./getwebextensions/) | 获取任务窗格的列表。 |
| [GetThreadedCommentAuthors](./getthreadedcommentauthors/) | 获取线程评论作者的列表。 |
| [IsRefreshAllConnections](./isrefreshallconnections/) | 指示在 MS Excel 中打开文件时是否刷新所有连接。 |
| [SetIsRefreshAllConnections](./setisrefreshallconnections/) | 指示在 MS Excel 中打开文件时是否刷新所有连接。 |
| [CreateRange](./createrange/) | 从范围地址创建 Range 对象。 |
| [CreateUnionRange](./createunionrange/) | 从范围地址创建 Range 对象。 |
| [GetNames](./getnames/) | 获取电子表格中所有 Name 对象的集合。 |
| [Get_Int](./get_int/) | 获取指定索引处的 Worksheet 元素。 |
| [Get_String](./get_string/) | 获取具有指定名称的 Worksheet 元素。 |
| [GetSheetByCodeName](./getsheetbycodename/) | 通过代码名称获取工作表。 |
| [GetActiveSheetName](./getactivesheetname/) | 表示打开电子表格时活动工作表的名称。 |
| [SetActiveSheetName](./setactivesheetname/) | 表示打开电子表格时活动工作表的名称。 |
| [GetActiveSheetIndex](./getactivesheetindex/) | 表示打开电子表格时活动工作表的索引。 |
| [SetActiveSheetIndex](./setactivesheetindex/) | 表示打开电子表格时活动工作表的索引。 |
| [SortNames](./sortnames/) | 对已定义的名称进行排序。 |
| [Insert_Int_SheetType](./insert_int_sheettype/) | 插入工作表。 |
| [Insert_Int_SheetType_String](./insert_int_sheettype_string/) | 插入工作表。 |
| [Add_SheetType](./add_sheettype/) | 向集合中添加工作表。 |
| [SwapSheet](./swapsheet/) | 交换两个工作表。 |
| [Add](./add/) | 向集合中添加工作表。 |
| [Add_String](./add_string/) | 向集合中添加工作表。 |
| [RegisterAddInFunction_String_String_Bool](./registeraddinfunction_string_string_bool/) | 向工作簿中添加加载项功能 |
| [RegisterAddInFunction_Int_String](./registeraddinfunction_int_string/) | 向工作簿中添加加载项功能 |
| [RemoveAt_String](./removeat_string/) | 删除具有指定名称的元素。 |
| [RemoveAt_Int](./removeat_int/) | 删除指定索引处的元素。 |
| [Clear](./clear/) | 清除所有工作表。 |
| [AddCopy_String](./addcopy_string/) | 向集合中添加工作表并从已存在的工作表复制数据。 |
| [AddCopy_Int](./addcopy_int/) | 向集合中添加工作表并从已存在的工作表复制数据。 |
| [AddCopy_WorksheetArray_stringArray](./addcopy_worksheetarray_stringarray/) | 复制一组工作表。 |
| [GetDxfs](./getdxfs/) | 获取主差异格式记录。 |
| [GetRangeByName_String](./getrangebyname_string/) | 通过预定义名称获取 Range 对象。 |
| [GetRangeByName_String_Int_Bool](./getrangebyname_string_int_bool/) | 通过预定义名称或表名获取 Range |
| [GetNamedRanges](./getnamedranges/) | 获取电子表格中所有预定义的命名范围。 |
| [GetNamedRangesAndTables](./getnamedrangesandtables/) | 获取电子表格中所有预定义的命名范围。 |
| [GetXmlMaps](./getxmlmaps/) | 获取并设置工作簿中的 XML 映射。 |
| [SetXmlMaps](./setxmlmaps/) | 获取并设置工作簿中的 XML 映射。 |
| [GetBuiltInDocumentProperties](./getbuiltindocumentproperties/) | 返回一个 DocumentProperty 集合，表示电子表格的所有内置文档属性。 |
| [GetCustomDocumentProperties](./getcustomdocumentproperties/) | 返回一个 DocumentProperty 集合，表示电子表格的所有自定义文档属性。 |
| [GetOleSize](./getolesize/) | 当工作簿文件用作 Ole 对象时，获取并设置显示尺寸。 |
| [SetOleSize_Object](./setolesize_object/) | 当工作簿文件用作 Ole 对象时，获取并设置显示尺寸。 |
| [SetOleSize_Int_Int_Int_Int](./setolesize_int_int_int_int/) | 当工作簿文件用作 Ole 对象时，设置显示尺寸。 |
| [GetExternalLinks](./getexternallinks/) | 表示工作簿中的外部链接。 |
| [GetPivotCaches](./getpivotcaches/) | 获取所有 PivotCache。 |
| [GetTableStyles](./gettablestyles/) | 获取 TableStyles 对象。 |
| [ClearPivottables](./clearpivottables/) | 从电子表格中清除数据透视表。 |
| [GetRevisionLogs](./getrevisionlogs/) | 表示修订日志。 |
| [RefreshPivotTables](./refreshpivottables/) | 刷新 Excel 文件中的所有数据透视表。 |
| [RefreshPivotTables_PivotTableRefreshOption](./refreshpivottables_pivottablerefreshoption/) | 刷新 Excel 文件中的所有数据透视表。 |
| [GetSensitivityLabels](./getsensitivitylabels/) | 表示所有敏感度标签。 |
| [GetCount](./getcount/) | 获取实例中包含的元素数量。 |
