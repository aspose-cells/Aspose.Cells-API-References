---
title: "RowCollection 类"
linktitle: "RowCollection"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "RowCollection 类。封装了在 Go 中表示 rowcollection 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/rowcollection/
---

## RowCollection class

收集表示工作表中各行的 <see cref="Row"/> 对象。

```go

type RowCollection struct  {
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
| [GetCount](./getcount/) | 获取此集合中行的数量。 |
| [GetEnumerator](./getenumerator/) | 获取一个遍历此集合中行的枚举器。 |
| [GetEnumerator_Bool_Bool](./getenumerator_bool_bool/) | 获取一个遍历此集合中行的枚举器。 |
| [GetRowByIndex](./getrowbyindex/) | 通过列表中的位置获取行对象。 |
| [Get](./get/) | 通过给定的行索引获取 Row 对象。如果该行索引对应的 Row 对象之前不存在，将会实例化它。 |
| [Clear](./clear/) | 清除所有行和单元格。 |
| [RemoveAt](./removeat/) | 移除此集合中指定索引（位置）的行项。 |
