---
title: SpreadsheetML2003SaveOptions.LimitAsXls
second_title: Aspose.Cells for .NET API Reference
description: SpreadsheetML2003SaveOptions property. Limit as xls the max row index is 65535 and the max column index is 255
type: docs
url: /net/aspose.cells/spreadsheetml2003saveoptions/limitasxls/
---
## SpreadsheetML2003SaveOptions.LimitAsXls property

Limit as xls, the max row index is 65535 and the max column index is 255.

```csharp
public bool LimitAsXls { get; set; }
```

### Examples

```csharp
// Called: LimitAsXls = true
[Test]
        public void Property_LimitAsXls()
        {
            caseName = "testCreateRange_Excel2007_004";
            Workbook workbook = new Workbook(FileFormatType.Xlsx);
            Cells cells = workbook.Worksheets[0].Cells;
            Aspose.Cells.Range range = cells.CreateRange("A1", "XFD1048576");
            range.Name = "testRange";

            checkCreateRange_Excel2007_001(workbook);
            workbook.Save(Constants.destPath + "testCreateRange.xlsx");
            workbook = new Workbook(Constants.destPath + "testCreateRange.xlsx");
            checkCreateRange_Excel2007_001(workbook);
            SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions()
            {
                LimitAsXls = true
            };
            workbook.Save(Constants.destPath + "testCreateRange.xml", saveOptions);
            workbook = new Workbook(Constants.destPath + "testCreateRange.xml");
            workbook.Save(Constants.destPath + "testCreateRange.xls"); 
        }
```

### See Also

* class [SpreadsheetML2003SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


