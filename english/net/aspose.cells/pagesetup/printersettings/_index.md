---
title: PageSetup.PrinterSettings
second_title: Aspose.Cells for .NET API Reference
description: PageSetup property. Gets and sets the settings of the default printer
type: docs
url: /net/aspose.cells/pagesetup/printersettings/
---
## PageSetup.PrinterSettings property

Gets and sets the settings of the default printer.

```csharp
public byte[] PrinterSettings { get; set; }
```

### Examples

```csharp
// Called: sheet.PageSetup.PrinterSettings = null;
[Test]
        public void Property_PrinterSettings()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet45347.xlsx");
            foreach (Worksheet sheet in workbook.Worksheets)
            {
                sheet.PageSetup.PrinterSettings = null;
            }
            workbook.Save(Constants.destPath + "CellsNet45347.xlsx");
            workbook = new Workbook(Constants.destPath + "CellsNet45347.xlsx");
            Assert.IsTrue(workbook.Worksheets[0].PageSetup.PrinterSettings == null);
            Assert.IsTrue(workbook.Worksheets[1].PageSetup.PrinterSettings == null);

        }
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


