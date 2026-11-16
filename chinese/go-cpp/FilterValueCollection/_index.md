---
title: "FilterValueCollection 类"
linktitle: "FilterValueCollection"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "FilterValueCollection 类。封装在 Go 中表示 filtervaluecollection 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/filtervaluecollection/
---

## FilterValueCollection class

表示多个筛选器的集合。

```go

type FilterValueCollection struct  {
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
| [GetMatchBlank](./getmatchblank/) | 指示是否按空白进行过滤。 |
| [SetMatchBlank](./setmatchblank/) | 指示是否按空白进行过滤。 |
| [Get](./get/) | 根据索引获取 FilterValue。 |
| [Add_String](./add_string/) | 添加标签过滤条件。 |
| [Add_DateTimeGroupingType_Int_Int_Int](./add_datetimegroupingtype_int_int_int/) | 添加日期过滤条件值。 |
| [Add_DateTimeGroupingType_Int_Int_Int_Int_Int_Int](./add_datetimegroupingtype_int_int_int_int_int_int/) | 添加日期时间过滤条件值。 |
| [GetCount](./getcount/) | 获取实例中包含的元素数量。 |
