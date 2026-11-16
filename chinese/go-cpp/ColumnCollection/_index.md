---
title: "ColumnCollection 类"
linktitle: "ColumnCollection"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "ColumnCollection 类。封装在 Go 中表示 columncollection 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/columncollection/
---

## ColumnCollection class

表示工作表中表示各个列（设置）的 <see cref="Column"/> 对象的集合。Column 对象仅表示整列的设置，如列宽、样式等，与对应列中是否存在非空单元格（数据）无关。此集合的 “Count” 仅表示已在该集合中实例化的 Column 对象的数量，也与工作表中是否存在非空单元格（数据）无关。

```go

type ColumnCollection struct  {
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
| [GetColumnByIndex](./getcolumnbyindex/) | 通过列表中的位置获取 Column 对象。 |
| [Get](./get/) | 通过列索引获取 Column 对象。如果给定列索引的 Column 对象之前不存在，将会实例化它。 |
| [GetCount](./getcount/) | 获取实例中包含的元素数量。 |
