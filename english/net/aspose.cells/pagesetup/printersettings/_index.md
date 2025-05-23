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
// Called: Assert.IsTrue(workbook.Worksheets[1].Charts[0].PageSetup.PrinterSettings == null);
public void PageSetup_Property_PrinterSettings()
{
    var workbook = new Workbook(Constants.sourcePath + "example.xls");
    Assert.AreEqual(workbook.Worksheets[0].Type, SheetType.Chart);
    Assert.IsTrue(workbook.Worksheets[1].Charts[0].PageSetup.PrinterSettings == null);
    Assert.AreEqual(2, workbook.Worksheets[1].Charts.Count);
    workbook.Save(Constants.destPath + "example.xls");
}
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


