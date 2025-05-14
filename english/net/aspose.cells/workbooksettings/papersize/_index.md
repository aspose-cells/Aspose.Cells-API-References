---
title: WorkbookSettings.PaperSize
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Gets and sets the default print paper size
type: docs
url: /net/aspose.cells/workbooksettings/papersize/
---
## WorkbookSettings.PaperSize property

Gets and sets the default print paper size.

```csharp
public PaperSizeType PaperSize { get; set; }
```

### Remarks

If there is no setting about paper size,MS Excel will use default printer's setting.

### Examples

```csharp
// Called: workbook.Settings.PaperSize = PaperSizeType.PaperA5;
public void WorkbookSettings_Property_PaperSize()
{
    LoadOptions options = new LoadOptions();
    options.SetPaperSize(PaperSizeType.PaperA5);
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls", options);
    Assert.AreEqual(PaperSizeType.PaperA5, workbook.Worksheets[0].PageSetup.PaperSize);
    workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    workbook.Settings.PaperSize = PaperSizeType.PaperA5;
    Assert.AreEqual(PaperSizeType.PaperA5, workbook.Worksheets[0].PageSetup.PaperSize);
}
```

### See Also

* enum [PaperSizeType](../../papersizetype/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


