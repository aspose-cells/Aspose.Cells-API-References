---
title: Cells.Rows
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Gets the collection of Row objects that represents the individual rows in this worksheet
type: docs
url: /net/aspose.cells/cells/rows/
---
## Cells.Rows property

Gets the collection of [`Row`](../../row/) objects that represents the individual rows in this worksheet.

```csharp
public RowCollection Rows { get; }
```

### Examples

```csharp
// Called: Assert.IsTrue(worksheet.Cells.Rows[0].IsHeightMatched);
public void Cells_Property_Rows()
{
    Workbook workbook = new Workbook();
    Worksheet worksheet = workbook.Worksheets[0];
    worksheet.Cells.SetColumnWidthPixel(0, 202);
    Cell cell = worksheet.Cells[0, 0];
    var cellStyle = cell.GetStyle();
    cellStyle.IsTextWrapped = true;
    cellStyle.Font.Name = "Calibri";
    cellStyle.Font.Size = 11;
    cell.SetStyle(cellStyle);

    cell.PutValue("aaaaaaaa aaaaaaaaaaa aaaaaaaa aaaaaaaa aaaaaaaaaaa aaaaaaaa aaaaaaaa aaaaaaaaaaa aaaaaaaa");

    AutoFitterOptions options = new AutoFitterOptions();
   // options.IsHeightMatched = false;
    worksheet.AutoFitRows(options);
    Assert.AreEqual(60,worksheet.Cells.GetRowHeightPixel(0));//It returns 60, whereas MS Excel shows 100 pixels
    Assert.IsTrue(worksheet.Cells.Rows[0].IsHeightMatched);
    workbook.Save(Constants.destPath + "example.xlsx", SaveFormat.Xlsx);
}
```

### See Also

* class [RowCollection](../../rowcollection/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


