---
title: PivotTable.RefreshDataOnOpeningFile
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Indicates whether Refresh Data when Opening File
type: docs
url: /net/aspose.cells.pivot/pivottable/refreshdataonopeningfile/
---
## PivotTable.RefreshDataOnOpeningFile property

Indicates whether Refresh Data when Opening File.

```csharp
public bool RefreshDataOnOpeningFile { get; set; }
```

### Examples

```csharp
// Called: pt.RefreshDataOnOpeningFile = false;
private void Property_RefreshDataOnOpeningFile(Worksheet ws)
        {
            foreach (PivotTable pt in ws.PivotTables)
            {
                pt.RefreshData();
                pt.CalculateData();
                pt.RefreshDataOnOpeningFile = false;
            }
            foreach (Chart chart in ws.Charts)
            {
                chart.RefreshPivotData();
                chart.Calculate();
            }
        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


