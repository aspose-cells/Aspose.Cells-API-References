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
// Called: int index = workbook.Worksheets.Names.Add("Test");
[Test]
        public void Property_Worksheets()
        {
            Workbook workbook = new Workbook(FileFormatType.Xlsx);
            int index = workbook.Worksheets.Names.Add("Test");
            workbook.Worksheets.Names[index].RefersTo = "=ADDRESS(ROW(),COLUMN())";

            workbook.Worksheets[0].Cells["C3"].Formula = "=Test";
            workbook.CalculateFormula();
            Assert.AreEqual("$C$3", workbook.Worksheets[0].Cells["C3"].Value);
        }
```

### See Also

* class [WorksheetCollection](../../worksheetcollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


