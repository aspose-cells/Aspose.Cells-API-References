---
title: "PivotFieldGroupOptions.GroupType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotFieldGroupOptions 属性。获取或设置透视字段的分组类型。仅适用于日期时间透视字段的分组"
type: docs
url: /zh/net/aspose.cells.pivot/pivotfieldgroupoptions/grouptype/
---
## PivotFieldGroupOptions.GroupType property

获取或设置枢轴字段的分组类型。仅适用于日期时间枢轴字段的分组。

```csharp
public PivotGroupByType GroupType { get; set; }
```

### 示例

```csharp
//init
PivotFieldGroupOptions pivotFieldGroupOptions = new PivotFieldGroupOptions();
// 按年份和月份一起分组
PivotGroupByType pivotGroupByType = pivotFieldGroupOptions.GroupType;
pivotGroupByType = PivotGroupByType.Years | PivotGroupByType.Months;
pivotFieldGroupOptions.GroupType = pivotGroupByType;
```

### 另请参见

* enum [PivotGroupByType](../../pivotgroupbytype/)
* class [PivotFieldGroupOptions](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


