---
title: PivotTable.IsAutoFormat
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Indicates whether the PivotTable report is automatically formatted. Checkbox autoformat table  which is in pivottable option for Excel 2003
type: docs
url: /net/aspose.cells.pivot/pivottable/isautoformat/
---
## PivotTable.IsAutoFormat property

Indicates whether the PivotTable report is automatically formatted. Checkbox "autoformat table " which is in pivottable option for Excel 2003

```csharp
public bool IsAutoFormat { get; set; }
```

### Examples

```csharp
// Called: pivotTable.IsAutoFormat = true; // Auto format columns?
private Worksheet PivotTable_Property_IsAutoFormat(Workbook workbook, string sourceData)
        {
            var pivotSheet = workbook.Worksheets.Add("Pivot Sheet");
            Console.Out.WriteLine(sourceData);
            var pivotTableIndex = pivotSheet.PivotTables.Add(
                sourceData,
                "A1",
                "PivotTable1");
            var pivotTable = pivotSheet.PivotTables[pivotTableIndex];
            pivotTable.ManualUpdate = false;
            pivotTable.IsAutoFormat = true; // Auto format columns?
            pivotTable.ShowInCompactForm();
            pivotTable.MissingItemsLimit = PivotMissingItemLimitType.None;

            //if the type is anything but PivotFieldType.Data it works
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Cats");
            //when you add multiple fields, it works
            //pivotTable.AddFieldToArea( PivotFieldType.Data, "Dogs" );

            pivotTable.CalculateData();
            pivotTable.RefreshDataOnOpeningFile = false;

            return pivotSheet;
        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


