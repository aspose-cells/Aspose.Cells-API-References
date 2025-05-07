---
title: PasteOptions.IgnoreLinksToOriginalFile
second_title: Aspose.Cells for .NET API Reference
description: PasteOptions property. Ingore links to the original file
type: docs
url: /net/aspose.cells/pasteoptions/ignorelinkstooriginalfile/
---
## PasteOptions.IgnoreLinksToOriginalFile property

Ingore links to the original file.

```csharp
public bool IgnoreLinksToOriginalFile { get; set; }
```

### Examples

```csharp
// Called: destRange.Copy(sourceRange, new PasteOptions { OnlyVisibleCells = false, IgnoreLinksToOriginalFile = true });
[Test]
        public void Property_IgnoreLinksToOriginalFile()
        {
            var sourceWrkbook = new Aspose.Cells.Workbook(Constants.sourcePath + "CellsNet52501.xlsm");
            var sourceRange = sourceWrkbook.Worksheets.GetRangeByName("Alx_PP_Income_Range");

            var workbook = new Workbook();
            workbook.CopyTheme(sourceRange.Worksheet.Workbook);

            var cells = workbook.Worksheets[0].Cells;

            var destRange = cells.CreateRange(0, 0, sourceRange.RowCount, sourceRange.ColumnCount);
            CopyOptions options = new CopyOptions();

            destRange.Copy(sourceRange, new PasteOptions { OnlyVisibleCells = false, IgnoreLinksToOriginalFile = true });
            Chart chart = workbook.Worksheets[0].Charts[0];
            Assert.AreEqual(chart.NSeries[0].Values, "{100,123.63419862,125.65372708,126.33007859,126.33007859,127.36842105,128.33769945}");
            Util.ReSave(workbook, SaveFormat.Xlsx);
            //workbook.Save(Constants.destPath + "CellsNet52501.xlsx");
        }
```

### See Also

* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


