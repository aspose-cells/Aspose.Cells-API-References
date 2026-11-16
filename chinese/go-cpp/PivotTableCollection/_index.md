---
title: "PivotTableCollection 类"
linktitle: "PivotTableCollection"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "PivotTableCollection 类。封装在 Go 中表示 pivottablecollection 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/pivottablecollection/
---

## PivotTableCollection class

表示指定工作表上所有 PivotTable 对象的集合。

```go

type PivotTableCollection struct  {
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
| [Dispose](./dispose/) | 执行应用程序定义的任务，涉及释放、释放或重置非托管资源。 |
| [Add_String_Int_Int](./add_string_int_int/) | 在指定的工作表行和列位置添加一个新的 PivotTable，使用默认选项。 |
| [Add_String_Int_Int_String_Bool_Bool](./add_string_int_int_string_bool_bool/) | 添加一个使用传统 Excel 97-2003 布局和样式的新 PivotTable。 |
| [Add_String_String_String_Bool_Bool](./add_string_string_string_bool_bool/) | 添加一个新的 PivotTable。 |
| [Add_PivotTable_String_String](./add_pivottable_string_string/) | 基于另一个 PivotTable 添加一个新的 PivotTable。 |
| [Add_PivotTable_Int_Int_String](./add_pivottable_int_int_string/) | 基于另一个 PivotTable 添加一个新的 PivotTable。 |
| [Add_stringArray_Bool_PivotPageFields_String_String](./add_stringarray_bool_pivotpagefields_string_string/) | 向集合中添加一个新的 PivotTable 对象，使用多个合并范围作为数据源。 |
| [Add_stringArray_Bool_PivotPageFields_Int_Int_String](./add_stringarray_bool_pivotpagefields_int_int_string/) | 向集合中添加一个新的 PivotTable 对象，使用多个合并范围作为数据源。 |
| [Get_Int](./get_int/) | 按索引获取 PivotTable 报表。 |
| [Get_String](./get_string/) | 按 PivotTable 的名称获取报表。 |
| [Get_Int_Int](./get_int_int/) | 按 PivotTable 的位置获取报表。 |
| [Clear](./clear/) | 清除所有 PivotTable。 |
| [Remove_PivotTable](./remove_pivottable/) | 删除指定的 PivotTable 并删除 PivotTable 数据。 |
| [Remove_PivotTable_Bool](./remove_pivottable_bool/) | 删除指定的 PivotTable。 |
| [RemoveAt_Int](./removeat_int/) | 删除指定索引处的 PivotTable 并删除 PivotTable 数据。 |
| [RemoveAt_Int_Bool](./removeat_int_bool/) | 删除指定索引处的 PivotTable。 |
| [GetCount](./getcount/) | 获取实例中包含的元素数量。 |
