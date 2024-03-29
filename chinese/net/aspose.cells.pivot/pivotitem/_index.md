---
title: PivotItem
second_title: Aspose.Cells for .NET API 参考
description: 表示 PivotField 报表中的项目
type: docs
weight: 4640
url: /zh/net/aspose.cells.pivot/pivotitem/
---
## PivotItem class

表示 PivotField 报表中的项目。

```csharp
public class PivotItem
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [Index](../../aspose.cells.pivot/pivotitem/index) { get; set; } | 获取枢轴字段中枢轴项的索引 |
| [IsHidden](../../aspose.cells.pivot/pivotitem/ishidden) { get; set; } | 获取和设置枢轴项目是否隐藏。 |
| [IsHideDetail](../../aspose.cells.pivot/pivotitem/ishidedetail) { get; set; } | 获取和设置透视项目是否隐藏细节。 |
| [Name](../../aspose.cells.pivot/pivotitem/name) { get; } | 获取数据透视项目的名称。 |
| [Position](../../aspose.cells.pivot/pivotitem/position) { set; } | 指定所有PivotItem中的位置索引，而不是同一父节点下的PivotItems。 |
| [PositionInSameParentNode](../../aspose.cells.pivot/pivotitem/positioninsameparentnode) { set; } | 指定同一父节点下PivotItems中的位置索引。 |
| [Value](../../aspose.cells.pivot/pivotitem/value) { get; } | 获取枢轴项的值 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [GetDateTimeValue](../../aspose.cells.pivot/pivotitem/getdatetimevalue)() | 获取pivot item的日期时间值 如果值为null，则返回DateTime.MinValue |
| [GetDoubleValue](../../aspose.cells.pivot/pivotitem/getdoublevalue)() | 获取pivot item的double值 如果值为null或者不是number，则返回0 |
| [GetStringValue](../../aspose.cells.pivot/pivotitem/getstringvalue)() | 获取pivot item的字符串值 如果值为null，则返回"" |
| [Move](../../aspose.cells.pivot/pivotitem/move)(int, bool) | 向上或向下移动项目 |

### 也可以看看

* 命名空间 [Aspose.Cells.Pivot](../../aspose.cells.pivot)
* 部件 [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
