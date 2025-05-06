---
title: PivotTable.ManualUpdate
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Indicates whether the PivotTable report is recalculated only at the users request
type: docs
url: /net/aspose.cells.pivot/pivottable/manualupdate/
---
## PivotTable.ManualUpdate property

Indicates whether the PivotTable report is recalculated only at the user's request.

```csharp
public bool ManualUpdate { get; set; }
```

### Examples

```csharp
// Called: pivotTable.ManualUpdate = false;
private Worksheet Property_ManualUpdate(Workbook workbook, string sourceData)
        {
            var pivotSheet = workbook.Worksheets.Add(&quot;Pivot Sheet&quot;);
            Console.Out.WriteLine(sourceData);
            var pivotTableIndex = pivotSheet.PivotTables.Add(
                sourceData,
                &quot;A1&quot;,
                &quot;PivotTable1&quot;);
            var pivotTable = pivotSheet.PivotTables[pivotTableIndex];
            pivotTable.ManualUpdate = false;
            pivotTable.IsAutoFormat = true; // Auto format columns?
            pivotTable.ShowInCompactForm();
            pivotTable.MissingItemsLimit = PivotMissingItemLimitType.None;

            //if the type is anything but PivotFieldType.Data it works
            pivotTable.AddFieldToArea(PivotFieldType.Data, &quot;Cats&quot;);
            //when you add multiple fields, it works
            //pivotTable.AddFieldToArea( PivotFieldType.Data, &quot;Dogs&quot; );

            pivotTable.CalculateData();
            pivotTable.RefreshDataOnOpeningFile = false;

            return pivotSheet;
        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


