---
title: Workbook.Worksheets
second_title: Aspose.Cells for .NET API Reference
description: Workbook property. Gets the WorksheetCollection collection in the spreadsheet
type: docs
url: /net/aspose.cells/workbook/worksheets/
---
## Workbook.Worksheets property

Gets the [`WorksheetCollection`](../../worksheetcollection/) collection in the spreadsheet.

```csharp
public WorksheetCollection Worksheets { get; }
```

### Return Value

[`WorksheetCollection`](../../worksheetcollection/) collection

### Examples

```csharp
// Called: sorter.Sort(workbook.Worksheets[1].Cells, CellArea.CreateCellArea("A2", "C6"));
public void Workbook_Property_Worksheets()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    DataSorter sorter = workbook.DataSorter;
    sorter.AddKey(1, SortOnType.CellColor, SortOrder.Descending, Color.Red);
    sorter.Sort(workbook.Worksheets[1].Cells, CellArea.CreateCellArea("A2", "C6"));
    Assert.AreEqual("2", workbook.Worksheets[1].Cells["B5"].StringValue);
    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
   sorter = workbook.DataSorter;
    sorter.AddKey(1, SortOnType.CellColor, SortOrder.Ascending, Color.Red);
    sorter.Sort(workbook.Worksheets[1].Cells, CellArea.CreateCellArea("A2", "C6"));
    Assert.AreEqual("2", workbook.Worksheets[1].Cells["B2"].StringValue);
    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [WorksheetCollection](../../worksheetcollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


