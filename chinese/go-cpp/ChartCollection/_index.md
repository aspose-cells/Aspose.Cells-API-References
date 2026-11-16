---
title: "ChartCollection 类"
linktitle: "ChartCollection"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "ChartCollection 类。封装在 Go 中表示 chartcollection 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/chartcollection/
---

## ChartCollection class

封装 <see cref="Chart"/> 对象的集合。

```go

type ChartCollection struct  {
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
| [AddFloatingChart](./addfloatingchart/) | 向集合中添加图表。 |
| [Add_ChartType_Int_Int_Int_Int](./add_charttype_int_int_int_int/) | 向集合中添加图表。 |
| [Add_Stream_String_Bool_Int_Int_Int_Int](./add_stream_string_bool_int_int_int_int/) | 使用预设模板添加图表。 |
| [Add_ChartType_String_Bool_Int_Int_Int_Int](./add_charttype_string_bool_int_int_int_int/) | 向集合中添加图表。 |
| [Get_Int](./get_int/) | 获取指定索引处的 Chart 元素。 |
| [Get_String](./get_string/) | 通过名称获取 chart。 |
| [RemoveAt](./removeat/) | 在特定索引处移除 chart。 |
| [Clear](./clear/) | 清除所有 chart。 |
| [GetCount](./getcount/) | 获取实例中包含的元素数量。 |
