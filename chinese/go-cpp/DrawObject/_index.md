---
title: "DrawObject 类"
linktitle: "DrawObject"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "DrawObject 类。封装表示 Go 中 drawobject 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/drawobject/
---

## DrawObject class

渲染时将初始化并返回 DrawObject。

```go

type DrawObject struct  {
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
| [GetCell](./getcell/) | 指示渲染时的 Cell 对象。可以访问单元格的所有属性。 |
| [GetShape](./getshape/) | 指示渲染时的 Shape 对象。可以访问形状的所有属性。 |
| [GetImageBytes](./getimagebytes/) | 指示渲染后 Chart、Shape 的图像字节。 |
| [GetType](./gettype/) | 指示 DrawObject 的类型。 |
| [GetCurrentPage](./getcurrentpage/) | 指示 DrawObject 的页索引。页索引从零开始。一个 Sheet 在渲染时包含多个页面。 |
| [GetTotalPages](./gettotalpages/) | 指示当前渲染的总页数。 |
| [GetSheetIndex](./getsheetindex/) | 指示 DrawObject 的当前 Sheet 索引。 |
