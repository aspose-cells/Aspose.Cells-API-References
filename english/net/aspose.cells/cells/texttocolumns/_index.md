---
title: Cells.TextToColumns
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Splits content in specified column into multiple columns
type: docs
url: /net/aspose.cells/cells/texttocolumns/
---
## Cells.TextToColumns method

Splits content in specified column into multiple columns..

```csharp
public int TextToColumns(int row, int column, int totalRows, TxtLoadOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | The row index. |
| column | Int32 | The column index. |
| totalRows | Int32 | The number of rows. |
| options | TxtLoadOptions | The split options. |

### Return Value

Total column count of the split values.

### Examples

```csharp
// Called: sheet.Cells.TextToColumns(1, 1, 3, options);
public void Cells_Method_TextToColumns()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Worksheet sheet = workbook.Worksheets[0];
    //Console.WriteLine(sheet.Cells.GetColumnWidthPixel(2));
    //sheet.AutoFitRows();
    TxtLoadOptions options = new TxtLoadOptions();
    options.Separator = ',';
    sheet.Cells.TextToColumns(1, 1, 3, options);
    Assert.AreEqual(sheet.Cells["B2"].StringValue,"a");
    Assert.AreEqual(sheet.Cells["C2"].StringValue, "b");
    workbook.Save(Constants.destPath + "dest.xlsx"); 
}
```

### See Also

* class [TxtLoadOptions](../../txtloadoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


