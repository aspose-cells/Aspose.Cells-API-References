---
title: TxtSaveOptions.ExportAllSheets
second_title: Aspose.Cells for .NET API Reference
description: TxtSaveOptions property. Indicates whether exporting all sheets to the text file. If it is false only export the activesheet just like MS Excel
type: docs
url: /net/aspose.cells/txtsaveoptions/exportallsheets/
---
## TxtSaveOptions.ExportAllSheets property

Indicates whether exporting all sheets to the text file. If it is false, only export the activesheet, just like MS Excel.

```csharp
public bool ExportAllSheets { get; set; }
```

### Remarks

The defult value is false.

### Examples

```csharp
// Called: saveOptions.ExportAllSheets = true;
[Test]
        public void Property_ExportAllSheets()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet48002.xlsx");
            TxtSaveOptions saveOptions = new TxtSaveOptions(SaveFormat.Csv);
            workbook.Save(Constants.destPath + "CellsNet48002.csv", saveOptions);
            workbook = new Workbook(Constants.destPath + "CellsNet48002.csv");
            Assert.AreEqual(2, workbook.Worksheets[0].Cells.MaxDataRow);

            workbook = new Workbook(Constants.sourcePath + "CellsNet48002.xlsx");
            saveOptions = new TxtSaveOptions(SaveFormat.Csv);
            saveOptions.ExportAllSheets = true;
            workbook.Save(Constants.destPath + "CellsNet48002.csv", saveOptions);
            workbook = new Workbook(Constants.destPath + "CellsNet48002.csv");
            Assert.AreEqual(6, workbook.Worksheets[0].Cells.MaxDataRow);
        }
```

### See Also

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


