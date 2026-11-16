---
title: "NameCollection 类"
linktitle: "NameCollection"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "NameCollection 类。封装在 Go 中表示 namecollection 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/namecollection/
---

## NameCollection class

表示电子表格中所有 <see cref="Name"/> 对象的集合。

```go

type NameCollection struct  {
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
| [Add](./add/) | 定义一个新名称。 |
| [Get_Int](./get_int/) | 获取指定索引处的 Name 元素。 |
| [Filter](./filter/) | 按作用域获取所有已定义的名称。 |
| [Get_String](./get_string/) | 获取具有指定名称的 Name 元素。 |
| [Remove_stringArray](./remove_stringarray/) | 删除一组名称 |
| [Remove_String](./remove_string/) | 删除该名称。 |
| [RemoveAt](./removeat/) | 删除特定索引处的名称。 |
| [Clear](./clear/) | 删除所有未被公式和数据源引用的已定义名称。如果已定义名称被引用，我们仅将 Name.ReferTo 设置为 null 并隐藏它们。 |
| [RemoveDuplicateNames](./removeduplicatenames/) | 删除重复的已定义名称 |
| [Sort](./sort/) | 对已定义名称进行排序。 |
| [GetCount](./getcount/) | 获取实例中包含的元素数量。 |
