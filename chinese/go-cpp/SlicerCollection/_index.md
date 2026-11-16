---
title: "SlicerCollection 类"
linktitle: "SlicerCollection"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "SlicerCollection 类。封装在 Go 中表示 slicercollection 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/slicercollection/
---

## SlicerCollection class

指定指定工作表上所有切片器对象的集合。

```go

type SlicerCollection struct  {
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
| [Get_Int](./get_int/) | 通过索引获取 Slicer。 |
| [Get_String](./get_string/) | 通过 slicer 的名称获取 Slicer。 |
| [Remove](./remove/) | 删除指定的 Slicer |
| [RemoveAt](./removeat/) | 删除位于指定索引的 Slicer |
| [Clear](./clear/) | 清除所有 Slicer。 |
| [Add_PivotTable_String_String](./add_pivottable_string_string/) | 使用 PivotTable 作为数据源添加新的 Slicer |
| [Add_PivotTable_Int_Int_String](./add_pivottable_int_int_string/) | 使用 PivotTable 作为数据源添加新的 Slicer |
| [Add_PivotTable_Int_Int_Int](./add_pivottable_int_int_int/) | 使用 PivotTable 作为数据源添加新的 Slicer |
| [Add_PivotTable_String_Int](./add_pivottable_string_int/) | 使用 PivotTable 作为数据源添加新的 Slicer |
| [Add_PivotTable_Int_Int_PivotField](./add_pivottable_int_int_pivotfield/) | 使用 PivotTable 作为数据源添加新的 Slicer |
| [Add_PivotTable_String_PivotField](./add_pivottable_string_pivotfield/) | 使用 PivotTable 作为数据源添加新的 Slicer |
| [Add_ListObject_Int_String](./add_listobject_int_string/) | 使用 ListObjet 作为数据源添加新的 Slicer |
| [Add_ListObject_ListColumn_String](./add_listobject_listcolumn_string/) | 使用 ListObjet 作为数据源添加新的 Slicer |
| [Add_ListObject_ListColumn_Int_Int](./add_listobject_listcolumn_int_int/) | 使用 ListObjet 作为数据源添加新的 Slicer |
| [GetCount](./getcount/) | 获取实例中包含的元素数量。 |
