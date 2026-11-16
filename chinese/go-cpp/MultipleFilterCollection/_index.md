---
title: "MultipleFilterCollection 类"
linktitle: "MultipleFilterCollection"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "MultipleFilterCollection 类。封装了在 Go 中表示 multiplefiltercollection 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/multiplefiltercollection/
---

## MultipleFilterCollection class

表示多个筛选器的集合。

```go

type MultipleFilterCollection struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewMultipleFilterCollection](./newmultiplefiltercollection/) | 从可转换为此对象的 Object 构造。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [ToObject](./toobject/) | 获取对象。 |
| [GetCount](./getcount/) | 获取过滤值的计数。 |
| [GetMatchBlank](./getmatchblank/) | 指示是否按空白进行过滤。 |
| [SetMatchBlank](./setmatchblank/) | 指示是否按空白进行过滤。 |
| [Get](./get/) | 获取 DateTimeGroupItem 或字符串值。 |
| [Add_String](./add_string/) | 添加标签过滤条件。 |
| [Add_DateTimeGroupingType_Int_Int_Int](./add_datetimegroupingtype_int_int_int/) | 添加日期过滤条件值。 |
| [Add_DateTimeGroupingType_Int_Int_Int_Int_Int_Int](./add_datetimegroupingtype_int_int_int_int_int_int/) | 添加日期时间过滤条件值。 |
| [GetEnumerator](./getenumerator/) | 获取过滤值的枚举器， |
