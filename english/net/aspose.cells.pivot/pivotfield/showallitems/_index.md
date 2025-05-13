---
title: PivotField.ShowAllItems
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Indicates whether all items displays in the PivotTable report even if they dont contain summary data. show items with no data The default value is false
type: docs
url: /net/aspose.cells.pivot/pivotfield/showallitems/
---
## PivotField.ShowAllItems property

Indicates whether all items displays in the PivotTable report, even if they don't contain summary data. show items with no data The default value is false.

```csharp
public bool ShowAllItems { get; set; }
```

### Examples

```csharp
// Called: pt.PageFields[0].ShowAllItems = true;
public void PivotField_Property_ShowAllItems()
{
    string filePath = Constants.PivotTableSourcePath + @"NET46033_";

    Workbook wb = new Workbook(filePath + "example.csv");
    Aspose.Cells.Range source = wb.Worksheets[0].Cells.CreateRange("A1", "C4");

    Workbook wb2 = new Workbook(filePath + "Sample_PivotTemplate_Original.xlsx");
    Aspose.Cells.Range dest = wb2.Worksheets["Data"].Cells.CreateRange("A1", "C4");
    dest.CopyData(source);
    PivotTable pt = wb2.Worksheets[0].PivotTables[0];
    pt.RefreshData();
    pt.CalculateData();
    pt.PageFields[0].ShowAllItems = true;
    pt.RefreshDataOnOpeningFile = true;

    wb2.Save(CreateFolder(filePath) + "out_Refresh.xlsx");

    pt.RefreshDataOnOpeningFile = false;

    wb2.Save(CreateFolder(filePath) + "out_noRefresh.xlsx");
}
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


