---
title: "DataBarAxisPosition 枚举"
linktitle: "DataBarAxisPosition"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "DataBarAxisPosition 枚举。封装表示 Go 中 databaraxisposition 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/databaraxisposition/
---

## DataBarAxisPosition Enum

指定带有条件格式的数据条的单元格范围的轴位置。

```go

type DataBarAxisPosition int32


```

## 字段

| 字段 | 描述 |
| --- | --- |
| [Automatic](./automatic/) | 根据范围内最小负值与最大正值的比例，在可变位置显示坐标轴。正值以从左到右的方向显示。负值以从右到左的方向显示。当所有值均为正或均为负时，不显示坐标轴。 |
| [Midpoint](./midpoint/) | 无论范围内的值集合如何，都在单元格的中点显示坐标轴。正值以从左到右的方向显示。负值以从右到左的方向显示。 |
| [None](./none/) | 不显示坐标轴，正负值均以从左到右的方向显示。 |
