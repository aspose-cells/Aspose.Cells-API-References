---
title: "DocumentPropertyCollection 类"
linktitle: "DocumentPropertyCollection"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "DocumentPropertyCollection 类。封装在 Go 中表示 documentpropertycollection 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/documentpropertycollection/
---

## DocumentPropertyCollection class

用于 <see cref="BuiltInDocumentPropertyCollection"/> 和 <see cref="CustomDocumentPropertyCollection"/> 集合的基类。

```go

type DocumentPropertyCollection struct  {
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
| [Get_Int](./get_int/) | 通过索引返回 DocumentProperty 对象。 |
| [Contains](./contains/) | 如果集合中存在具有指定名称的属性，则返回 true。 |
| [IndexOf](./indexof/) | 通过名称获取属性的索引。 |
| [Remove](./remove/) | 从集合中删除具有指定名称的属性。 |
| [RemoveAt](./removeat/) | 删除指定索引处的属性。 |
| [Get_String](./get_string/) | 通过属性名称返回 DocumentProperty 对象。 |
| [GetCount](./getcount/) | 获取实例中包含的元素数量。 |
