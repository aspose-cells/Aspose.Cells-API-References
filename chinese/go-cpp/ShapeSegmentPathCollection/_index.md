---
title: "ShapeSegmentPathCollection 类"
linktitle: "ShapeSegmentPathCollection"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "ShapeSegmentPathCollection 类。封装在 Go 中表示 shapesegmentpathcollection 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/shapesegmentpathcollection/
---

## ShapeSegmentPathCollection class

表示由一系列移动、直线和曲线组成的创建路径，组合后形成几何形状。

```go

type ShapeSegmentPathCollection struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewShapeSegmentPathCollection](./newshapesegmentpathcollection/) | 默认构造函数。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [Add](./add/) | 在创建路径中添加段路径。 |
| [Get](./get/) | 获取 ShapeSegmentPath 对象。 |
| [GetCount](./getcount/) | 获取实例中包含的元素数量。 |
