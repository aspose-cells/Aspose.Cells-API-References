---
title: SetBorderPosition
second_title: Aspose.Cells for .NET API 参考
description: 表示要设置的单元格范围的边框位置
type: docs
weight: 900
url: /zh/net/aspose.cells.gridweb/setborderposition/
---
## SetBorderPosition enumeration

表示要设置的单元格范围的边框位置。

```csharp
public enum SetBorderPosition
```

### 价值观

| 姓名 | 价值 | 描述 |
| --- | --- | --- |
| Top | `0` | 上边框 |
| Bottom | `1` | 底部边框 |
| Left | `2` | 左边框 |
| Right | `3` | 右边框 |
| HorizontalMiddle | `4` | 底部边框 |
| VerticalMiddle | `5` | 水平中间边框 |
| Outline | `6` | 垂直中间边框 |
| Cross | `7` | 跨境 |
| None | `8` | 无边框 |

### 例子

```csharp
[C#]
	GridWeb1.WebWorksheets[0].Cells.SetBorders(0, 0, 5, 8, SetBorderPosition.Outline, borderStyle1);

[VB]
	GridWeb1.WebWorksheets(0).Cells.SetBorders(0, 0, 5, 8, SetBorderPosition.Outline, borderStyle1)
```

### 也可以看看

* 命名空间 [Aspose.Cells.GridWeb](../../aspose.cells.gridweb)
* 部件 [Aspose.Cells.GridWeb](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->
