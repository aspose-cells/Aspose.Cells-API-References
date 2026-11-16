---
title: "OleObjectCollection 类"
linktitle: "OleObjectCollection"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "OleObjectCollection 类。封装在 Go 中表示 oleobjectcollection 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/oleobjectcollection/
---

## OleObjectCollection class

表示嵌入的 OLE 对象。

```go

type OleObjectCollection struct  {
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
| [Add_Int_Int_Int_Int_Stream](./add_int_int_int_int_stream/) | 向集合中添加一个 OleObject。 |
| [Add_Int_Int_Int_Int_Stream_String](./add_int_int_int_int_stream_string/) | 向集合中添加一个链接的 OleObject。 |
| [Get](./get/) | 获取指定索引处的 OleObject 元素。 |
| [Clear](./clear/) | 移除所有嵌入的 OLE 对象。 |
| [RemoveAt](./removeat/) | 移除指定索引处的元素。 |
| [GetCount](./getcount/) | 获取实例中包含的元素数量。 |
