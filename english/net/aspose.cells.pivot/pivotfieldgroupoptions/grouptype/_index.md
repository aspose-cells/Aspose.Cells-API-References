---
title: PivotFieldGroupOptions.GroupType
second_title: Aspose.Cells for .NET API Reference
description: PivotFieldGroupOptions property. Gets or sets the grouping type for pivot field. Only for grouping date time pivot field
type: docs
url: /net/aspose.cells.pivot/pivotfieldgroupoptions/grouptype/
---
## PivotFieldGroupOptions.GroupType property

Gets or sets the grouping type for pivot field. Only for grouping date time pivot field.

```csharp
public PivotGroupByType GroupType { get; set; }
```

### Examples

```csharp
//init
PivotFieldGroupOptions pivotFieldGroupOptions = new PivotFieldGroupOptions();
// Group by year and month together
PivotGroupByType pivotGroupByType = pivotFieldGroupOptions.GroupType;
pivotGroupByType = PivotGroupByType.Years | PivotGroupByType.Months;
pivotFieldGroupOptions.GroupType = pivotGroupByType;
```

### See Also

* enum [PivotGroupByType](../../pivotgroupbytype/)
* class [PivotFieldGroupOptions](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


