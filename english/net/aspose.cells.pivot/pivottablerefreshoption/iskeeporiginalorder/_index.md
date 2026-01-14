---
title: PivotTableRefreshOption.IsKeepOriginalOrder
second_title: Aspose.Cells for .NET API Reference
description: PivotTableRefreshOption property. Indicates whether to keep pivot items original order as old data source
type: docs
url: /net/aspose.cells.pivot/pivottablerefreshoption/iskeeporiginalorder/
---
## PivotTableRefreshOption.IsKeepOriginalOrder property

Indicates whether to keep pivot items' original order as old data source.

```csharp
public bool IsKeepOriginalOrder { get; set; }
```

### Remarks

Only applicable for the pivot field which is not sorted. When refreshing such kind of pivot field, Ms Excel keeps the original order of old data source. Default value of this property is true, representing the same behavior with Ms Excel. If user needs the pivot field to be refreshed completely as the data in the new data source, this property should be set as false.

### See Also

* class [PivotTableRefreshOption](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


